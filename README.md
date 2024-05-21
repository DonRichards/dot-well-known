# Draft .well-known
Concept idea for a Drupal modules to add Well-Known Uniform Resource Identifiers

## Breakdown of key elements within the example files
- .well-known/aicrawler file: [Explanation of Key Elements](Explanation_of_Key_Elements.md) 
- .well-known/ai-plugin.txt file [copied from](https://github.com/openai/chatgpt-retrieval-plugin/tree/main)
## List
- [https://en.wikipedia.org/wiki/Well-known_URI](https://en.wikipedia.org/wiki/Well-known_URI)

## Idea:
`well-known/` subdirectory is defined by [RFC8615](https://www.rfc-editor.org/rfc/rfc8615) Request for Comments (RFC) memorandum published by the Internet Engineering Task Force (IETF)

> It is increasingly common for Web-based protocols to require the discovery of policy or other information about a host ("site-wide metadata") before making a request. For example, the Robots Exclusion Protocol http://www.robotstxt.org/ specifies a way for automated processes to obtain permission to access resources; likewise, the Platform for Privacy Preferences [W3C.REC-P3P-20020416] tells user-agents how to discover privacy policy beforehand.
>
> While there are several ways to access per-resource metadata (e.g., HTTP headers, WebDAV's PROPFIND [RFC4918]), the perceived overhead (either in terms of client-perceived latency and/or deployment difficulties) associated with them often precludes their use in these scenarios.
> 
> When this happens, it is common to designate a "well-known location" for such data, so that it can be easily located. However, this approach has the drawback of risking collisions, both with other such designated "well-known locations" and with pre-existing resources.
>
> To address this, this memo defines a path prefix in HTTP(S) URIs for these "well-known locations", /.well-known/. Future specifications that need to define a resource for such site-wide metadata can register their use to avoid collisions and minimise impingement upon sites' URI space.

### Examples:
* /.well-known/apple-app-site-association is for [IOS universal links](https://developer.apple.com/library/ios/documentation/General/Conceptual/AppSearch/UniversalLinks.html)
* /.well-known/assetlinks.json is an [(Android) Digital Asset Link](https://developers.google.com/digital-asset-links/v1/getting-started)
* /.well-known/secruity.txt is a way for websites to [define security policies](https://github.com/securitytxt/security-txt/blob/master/archived/rfc9116.txt)

### More Examples:
* https://www.facebook.com/.well-known/security.txt


Full list of Well-Known URIs : https://www.iana.org/assignments/well-known-uris/well-known-uris.xhtml


