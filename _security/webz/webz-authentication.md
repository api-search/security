---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Webz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webz.io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Webz.io
provider_slug: webz
scheme_count: 3
schemes:
- applies_to:
  - https://api.webz.io/cyberFilter
  - https://api.webz.io/cyberSeg
  - https://api.webz.io/breaches
  - https://api.webz.io/breachCatalog
  - https://api.webz.io/reviewFilter
  - https://api.webz.io/reviewSeg
  - https://api.webz.io/firehose
  - https://app.webz.io/setArchiveQuery
  - https://app.webz.io/confirmArchiveQuery
  - https://app.webz.io/getArchiveOrderStatus
  - https://api.webz.io/api/news
  - https://api.webz.io/api/blogs
  - https://api.webz.io/api/forums
  description: The API token as a query parameter. This is the only documented method for the Cyber API, the Data Breaches API, the Reviews API, the Archive API and the Firehose FH API.
  id: api_token_query
  in: query
  name: token
  type: apiKey
- applies_to:
  - https://api.webz.io/api/news/context
  - https://api.webz.io/api/news
  - https://api.webz.io/api/blogs
  - https://api.webz.io/api/forums
  - https://news-search-mcp.webz.io/mcp
  description: Authorization Bearer header carrying the same API token. Documented as the RECOMMENDED method for the News Search API and as an alternative for News/Blogs/Forums. Not documented for Cyber, Data Breaches, Reviews, Archive or Firehose.
  id: api_token_bearer
  scheme: bearer
  type: http
- applies_to:
  - https://news-search-mcp.webz.io/mcp
  authorization_endpoint: https://news-search-mcp.webz.io/authorize
  description: RFC 8414 authorization-server metadata in front of the News Search MCP endpoint, used by Claude.ai and ChatGPT connectors. PKCE S256 required; dynamic client registration (RFC 7591) is advertised. The provider's own instructions say to leave Client ID and Secret empty and paste the Webz token on the authorize page, so the identity behind the OAuth grant is still the API token.
  flow: authorizationCode
  id: mcp_oauth
  registration_endpoint: https://news-search-mcp.webz.io/register
  scopes:
  - mcp
  token_endpoint: https://news-search-mcp.webz.io/token
  type: oauth2
slug: webz-authentication
source_filename: webz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.webz.io/docs/webz/news-blogs-forums-endpoints,\n  https://docs.webz.io/docs/webz/cyber-api-endpoints,\n  https://docs.webz.io/docs/webz/data-breach-endpoints,\n  https://docs.webz.io/docs/webz/reviews-api-endpoints,\n  https://docs.webz.io/docs/webz/news-search-api-endpoints,\n  https://docs.webz.io/docs/webz/news-search-api-mcp,\n  https://news-search-mcp.webz.io/.well-known/oauth-authorization-server\ndocs: https://docs.webz.io/docs/webz/news-blogs-forums-endpoints\nsummary: >-\n  One account token authenticates every Webz.io product. There is no OAuth on the REST APIs and no\n  per-product credential — access is granted by attaching product permissions to the single token,\n  which is why calling an endpoint you are not subscribed to returns 401 with a permission error\n  rather than 403. The only OAuth surface Webz.io operates is in front of the News Search MCP server,\n  and the provider documents that\
  \ flow as a wrapper that still ends in pasting the same API token.\nschemes:\n- id: api_token_query\n  type: apiKey\n  in: query\n  name: token\n  description: >-\n    The API token as a query parameter. This is the only documented method for the Cyber API, the\n    Data Breaches API, the Reviews API, the Archive API and the Firehose FH API.\n  applies_to:\n  - https://api.webz.io/cyberFilter\n  - https://api.webz.io/cyberSeg\n  - https://api.webz.io/breaches\n  - https://api.webz.io/breachCatalog\n  - https://api.webz.io/reviewFilter\n  - https://api.webz.io/reviewSeg\n  - https://api.webz.io/firehose\n  - https://app.webz.io/setArchiveQuery\n  - https://app.webz.io/confirmArchiveQuery\n  - https://app.webz.io/getArchiveOrderStatus\n  - https://api.webz.io/api/news\n  - https://api.webz.io/api/blogs\n  - https://api.webz.io/api/forums\n- id: api_token_bearer\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization Bearer header carrying the same API token. Documented as the\
  \ RECOMMENDED method\n    for the News Search API and as an alternative for News/Blogs/Forums. Not documented for Cyber,\n    Data Breaches, Reviews, Archive or Firehose.\n  applies_to:\n  - https://api.webz.io/api/news/context\n  - https://api.webz.io/api/news\n  - https://api.webz.io/api/blogs\n  - https://api.webz.io/api/forums\n  - https://news-search-mcp.webz.io/mcp\n- id: mcp_oauth\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    RFC 8414 authorization-server metadata in front of the News Search MCP endpoint, used by\n    Claude.ai and ChatGPT connectors. PKCE S256 required; dynamic client registration (RFC 7591)\n    is advertised. The provider's own instructions say to leave Client ID and Secret empty and paste\n    the Webz token on the authorize page, so the identity behind the OAuth grant is still the API token.\n  authorization_endpoint: https://news-search-mcp.webz.io/authorize\n  token_endpoint: https://news-search-mcp.webz.io/token\n  registration_endpoint:\
  \ https://news-search-mcp.webz.io/register\n  scopes:\n  - mcp\n  applies_to:\n  - https://news-search-mcp.webz.io/mcp\ntoken_acquisition:\n  where: https://app.webz.io/playground/dashboard\n  self_service: true\n  note: >-\n    A verified account with a positive credit balance is required. News API Lite issues a free\n    non-commercial token through https://webz.io/products/news-api#lite.\npermissions_model:\n  style: per-product entitlement attached to the token\n  documented_permissions:\n  - api_news\n  known_products:\n  - News / Blogs / Forums\n  - Reviews\n  - Cyber (dark web)\n  - Data Breaches\n  - Archive\n  - Firehose (FH API)\n  - News Search\n  escalation: >-\n    Adding a product is a sales/support action — support@webz.io for News/Blogs/Forums and Reviews,\n    sales@webz.io for Cyber, Data Breaches and Archive. There is no self-service upgrade path\n    documented for the dark-web products.\n  data_breach_extras:\n  - Domain authorization — a token may only search domains\
  \ authorized for it. A newly queried domain\n    is authorized automatically and takes ~20 seconds to index on first request; a domain with over\n    ~1,000,000 records in the past year is blocked with 403 until support enables it.\n  - A view-password permission controls whether the password field is returned in full or masked\n    (for example pa****23).\nfailure_modes:\n- status: 401\n  when: Missing or unknown token, or the account lacks the product permission for that endpoint.\n  body: '{ \"detail\": \"Unknown API token\" }'\n- status: 401\n  when: Cyber API without the Cyber permission. Note /cyberSeg returns 429 rather than 401 in this case.\n- status: 402\n  when: News Search — insufficient credits. Data Breaches — the account email is not verified.\n- status: 403\n  when: Account inactive, blocked, or trial ended; also an unauthorized or safeguard-blocked breach domain.\nwarnings:\n- The token travels in the query string on most products, so it lands in access logs, browser\n\
  \  history and any shared URL. The provider's own MCP guidance warns \"never commit your token to git\n  or put it in a URL\", which the query-parameter auth on the other six products directly contradicts.\n- Opening https://news-search-mcp.webz.io/mcp in a browser returns 401 by design.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webz/refs/heads/main/authentication/webz-authentication.yml
summary_line: 3 schemes
tags:
- news-data
- web-data
- web-scraping
- dark-web
- deep-web
- cybersecurity
- threat-intelligence
- data-breach
- pii-monitoring
- osint
- reviews-data
- ai-training-data
- media-monitoring
---
