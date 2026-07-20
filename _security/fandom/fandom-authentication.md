---
api_key_in: []
auth_types:
- session
- oauth2
- oauth1
description: ''
kind: authentication
layout: security
method: searched
name: Fandom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fandom secures its APIs with session, oauth2, and oauth1 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fandom
provider_slug: fandom
scheme_count: 5
schemes:
- description: Read modules (query, parse, opensearch, feed*) are available anonymously. Public read access is the default for content wikis; some private wikis gate reads behind login.
  name: AnonymousRead
  type: none
- description: All write actions (edit, upload, move, delete, etc.) require a CSRF token obtained from action=query&meta=tokens&type=csrf, plus an authenticated session cookie. Distinct token types exist (csrf, login, createaccount, patrol, rollback, userrights, watch, deleteglobalaccount).
  name: CsrfToken
  type: token
- description: Interactive/username-password login via action=clientlogin using AuthManager (the modern replacement for the legacy action=login). Establishes a session cookie carried on subsequent write requests.
  name: ClientLogin
  type: session
- description: Scoped, revocable credentials created at Special:BotPasswords for automated clients. Used with action=login (or clientlogin) to obtain a bot session with a restricted grant set, without exposing the account password.
  name: BotPassword
  type: session
- description: MediaWiki Extension:OAuth exposes OAuth 1.0a and OAuth 2.0 authorization at Special:OAuth for registered consumers, issuing owner-only or full authorization-code tokens with grant-based scopes. Availability of the OAuth consumer registration flow varies by Fandom deployment.
  flows:
  - authorizationUrl: https://community.fandom.com/wiki/Special:OAuth/authorize
    flow: authorizationCode
    tokenUrl: https://community.fandom.com/wiki/Special:OAuth/token
  name: OAuth
  type: oauth2
slug: fandom-authentication
source_filename: fandom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.mediawiki.org/wiki/API:Authentication\nnote: >-\n  Fandom runs MediaWiki 1.43.9 (confirmed live via\n  api.php?action=query&meta=siteinfo). It exposes the standard MediaWiki Action\n  API authentication surface. No bespoke Fandom auth spec is published; this\n  profile is grounded in the confirmed MediaWiki generator and the upstream\n  MediaWiki authentication documentation.\nsummary:\n  types:\n  - session\n  - oauth2\n  - oauth1\n  token_based: true\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  anonymous_read: true\nschemes:\n- name: AnonymousRead\n  type: none\n  description: >-\n    Read modules (query, parse, opensearch, feed*) are available anonymously.\n    Public read access is the default for content wikis; some private wikis gate\n    reads behind login.\n- name: CsrfToken\n  type: token\n  description: >-\n    All write actions (edit, upload, move, delete, etc.) require a CSRF token\n\
  \    obtained from action=query&meta=tokens&type=csrf, plus an authenticated\n    session cookie. Distinct token types exist (csrf, login, createaccount,\n    patrol, rollback, userrights, watch, deleteglobalaccount).\n- name: ClientLogin\n  type: session\n  description: >-\n    Interactive/username-password login via action=clientlogin using AuthManager\n    (the modern replacement for the legacy action=login). Establishes a session\n    cookie carried on subsequent write requests.\n- name: BotPassword\n  type: session\n  description: >-\n    Scoped, revocable credentials created at Special:BotPasswords for automated\n    clients. Used with action=login (or clientlogin) to obtain a bot session\n    with a restricted grant set, without exposing the account password.\n- name: OAuth\n  type: oauth2\n  description: >-\n    MediaWiki Extension:OAuth exposes OAuth 1.0a and OAuth 2.0 authorization at\n    Special:OAuth for registered consumers, issuing owner-only or full\n    authorization-code\
  \ tokens with grant-based scopes. Availability of the OAuth\n    consumer registration flow varies by Fandom deployment.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://community.fandom.com/wiki/Special:OAuth/authorize\n    tokenUrl: https://community.fandom.com/wiki/Special:OAuth/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fandom/refs/heads/main/authentication/fandom-authentication.yml
summary_line: session/oauth2/oauth1 · 5 schemes
tags:
- Company
- Consumer
- Wiki
- MediaWiki
- Media
- Entertainment
- Community
- Content
- Fan Community
---
