## Appendix B: Content Negotiation .HTACCESS (Apache) Example {#appendix-b-content-negotiation-htaccess-apache-example}

**Editor’s note:** This shortened example is provided for documentation purposes only and only shows how this can be accomplished using an Apache web server. Other web servers could be used such as NGINX. Please refer to the specific type of documentation for other web servers on how to address content negotiation and URL rewriting.

```
Options +FollowSymLinks
RewriteEngine on

# vocabulary dataset
# ---------------------------
# Rewrite rule to serve HTML content from the vocabulary IRI if requested
RewriteCond %{HTTP_ACCEPT} !application/rdf\+xml.*(text/html|application/xhtml\+xml)
RewriteCond %{HTTP_ACCEPT} text/html [OR]
RewriteCond %{HTTP_ACCEPT} application/xhtml\+xml [OR]
RewriteCond %{HTTP_USER_AGENT} ^Mozilla/.*
RewriteRule ^cmi5$ http://example.com/datasets/cmi5/index.html [R=303]

# Rewrite rule to serve JSON-LD content from the vocabulary URI if requested
RewriteCond %{HTTP_ACCEPT} application/ld\+json
RewriteRule ^cmi5$ http://example.com/datasets/cmi5.jsonld [R=303]

# verbs & activity types catch all IRIs
# ---------------------------
# Rewrite rule to serve HTML content from the vocabulary term IRI if requested
RewriteCond %{HTTP_ACCEPT} !application/rdf\+xml.*(text/html|application/xhtml\+xml)
RewriteCond %{HTTP_ACCEPT} text/html [OR]
RewriteCond %{HTTP_ACCEPT} application/xhtml\+xml [OR]
RewriteCond %{HTTP_USER_AGENT} ^Mozilla/.*
RewriteRule ^cmi5/([a-z-]+)$ http://example.com/datasets/cmi5/#$1 [R=303,NE]

# Rewrite rule to serve JSON-LD content from the vocabulary term IRI if requested
RewriteCond %{HTTP_ACCEPT} application/ld\+json
RewriteRule ^cmi5/[a-z-]+$ http://example.com/datasets/cmi5.jsonld [R=303]
```
*Figure 11\. Example of .htaccess (assuming the identifier base pattern is https://w3id.org/xapi/cmi5)*