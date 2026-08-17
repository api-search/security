---
api_key_in: []
auth_types:
- none
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Sundaysky Authentication
name_suffix: Authentication
oauth_flows: []
overview: SundaySky secures its APIs with none and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SundaySky
provider_slug: sundaysky
scheme_count: 3
schemes:
- applies_to: https://apis.sundaysky.com/get-video/player-session/{sundayskyVideoId}
  description: The SundaySky Video API documents no Authorization header, API key, or token. The only credential in the documented request is the SundaySky Video ID embedded in the URL path — a capability URL. The endpoint is designed to be called from a page or server that already holds the video's embed snippet, and the account is resolved server-side from the video ID.
  documented_headers:
  - name: Content-Type
    required: true
    value: application/json
  - description: Optional. Lets SundaySky determine the viewer's operating system, device type, and browser type for correct rendering and analytics attribution.
    name: User-Agent
    required: false
  evidence:
  - kind: docs
    note: The article's "Getting the API URL" section lists Headers as Mandatory (Content-Type) and Optional (User-Agent) only — no auth header is documented.
    url: https://help.sundaysky.com/hc/en-us/articles/6000894076957-Using-the-SundaySky-API-to-Connect-Data
  - fetched: '2026-08-13'
    http_status: 500
    kind: probe
    note: An unauthenticated POST reaches application logic rather than being rejected at an auth boundary — the response is a parameter-validation error naming accountId/programId/service/stage, not a 401/403. This confirms no bearer credential is required on this route.
    url: https://apis.sundaysky.com/get-video/player-session/00000000
  name: video-id-capability-url
  surface: api
  type: none
- availability: Plan-dependent — included on some plans, offered as a paid add-on on others. Enabled by SundaySky on request via the customer's Success Manager, not self-service.
  description: Single Sign-On to the SundaySky platform (Studio, Video Page, Analytics) via the customer's own Identity Provider. SundaySky acts as the Service Provider and supplies a SAML XML metadata file containing its entity ID, public certificate, and login/redirect URL. The customer returns their IdP SSO URL and X.509 certificate, or an IdP metadata endpoint URL.
  docs: https://help.sundaysky.com/hc/en-us/articles/27307608733981-Enabling-Single-Sign-On-SSO-for-Your-SundaySky-Account
  name: saml-sso
  provisioning: manual
  provisioning_note: SSO is used for authentication only; it does not provision users. All users must be created manually in the platform by an Account owner and assigned a user type before they can log in via SSO.
  surface: platform
  type: saml
  version: SAML 2.0
- description: Username and password login at https://app.sundaysky.com/ for accounts not configured for SSO, with a self-service password reset flow.
  docs: https://help.sundaysky.com/hc/en-us/articles/7302748637597-If-You-Forgot-Your-Password
  name: password
  surface: platform
  type: password
slug: sundaysky-authentication
source_filename: sundaysky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.sundaysky.com/hc/en-us/articles/6000894076957-Using-the-SundaySky-API-to-Connect-Data\ndocs: https://help.sundaysky.com/hc/en-us/articles/27307608733981-Enabling-Single-Sign-On-SSO-for-Your-SundaySky-Account\nnote: >-\n  SundaySky publishes no OpenAPI, so no securitySchemes could be derived\n  mechanically (derive-authentication.py returned 0 profiles). This profile is\n  read from the provider's own help-center documentation and confirmed against a\n  live probe of the documented endpoint.\n\nsummary:\n  types:\n  - none\n  - saml\n  api_key_in: []\n  oauth2_flows: []\n  oauth2_supported: false\n  oauth2_note: >-\n    SundaySky states explicitly that OAuth is not supported for platform\n    authentication. No scopes/ artifact is emitted for this provider.\n\nschemes:\n- name: video-id-capability-url\n  surface: api\n  type: none\n  applies_to: https://apis.sundaysky.com/get-video/player-session/{sundayskyVideoId}\n\
  \  description: >-\n    The SundaySky Video API documents no Authorization header, API key, or token.\n    The only credential in the documented request is the SundaySky Video ID\n    embedded in the URL path — a capability URL. The endpoint is designed to be\n    called from a page or server that already holds the video's embed snippet,\n    and the account is resolved server-side from the video ID.\n  documented_headers:\n  - name: Content-Type\n    required: true\n    value: application/json\n  - name: User-Agent\n    required: false\n    description: >-\n      Optional. Lets SundaySky determine the viewer's operating system, device\n      type, and browser type for correct rendering and analytics attribution.\n  evidence:\n  - kind: docs\n    url: https://help.sundaysky.com/hc/en-us/articles/6000894076957-Using-the-SundaySky-API-to-Connect-Data\n    note: >-\n      The article's \"Getting the API URL\" section lists Headers as Mandatory\n      (Content-Type) and Optional (User-Agent)\
  \ only — no auth header is documented.\n  - kind: probe\n    url: https://apis.sundaysky.com/get-video/player-session/00000000\n    http_status: 500\n    fetched: '2026-08-13'\n    note: >-\n      An unauthenticated POST reaches application logic rather than being\n      rejected at an auth boundary — the response is a parameter-validation\n      error naming accountId/programId/service/stage, not a 401/403. This\n      confirms no bearer credential is required on this route.\n\n- name: saml-sso\n  surface: platform\n  type: saml\n  version: SAML 2.0\n  description: >-\n    Single Sign-On to the SundaySky platform (Studio, Video Page, Analytics) via\n    the customer's own Identity Provider. SundaySky acts as the Service Provider\n    and supplies a SAML XML metadata file containing its entity ID, public\n    certificate, and login/redirect URL. The customer returns their IdP SSO URL\n    and X.509 certificate, or an IdP metadata endpoint URL.\n  provisioning: manual\n  provisioning_note:\
  \ >-\n    SSO is used for authentication only; it does not provision users. All users\n    must be created manually in the platform by an Account owner and assigned a\n    user type before they can log in via SSO.\n  availability: >-\n    Plan-dependent — included on some plans, offered as a paid add-on on others.\n    Enabled by SundaySky on request via the customer's Success Manager, not\n    self-service.\n  docs: https://help.sundaysky.com/hc/en-us/articles/27307608733981-Enabling-Single-Sign-On-SSO-for-Your-SundaySky-Account\n\n- name: password\n  surface: platform\n  type: password\n  description: >-\n    Username and password login at https://app.sundaysky.com/ for accounts not\n    configured for SSO, with a self-service password reset flow.\n  docs: https://help.sundaysky.com/hc/en-us/articles/7302748637597-If-You-Forgot-Your-Password\n\nnot_supported:\n- protocol: oauth2\n  evidence: >-\n    \"SundaySky supports identity providers that use the SAML 2.0 protocol for\n    authentication.\
  \ OAuth is not currently supported.\" — Enabling Single Sign-On\n    (SSO) for Your SundaySky Account, retrieved 2026-08-13.\n- protocol: openid-connect\n  evidence: >-\n    No OIDC discovery document is served. /.well-known/openid-configuration\n    returns 404 on sundaysky.com and 403 on apis.sundaysky.com; the 200 observed\n    on app./studio. is an SPA catch-all HTML shell, not a document. See\n    well-known/sundaysky-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sundaysky/refs/heads/main/authentication/sundaysky-authentication.yml
summary_line: none/saml · 3 schemes
tags:
- Company
- Video
- Personalization
- Video Personalization
- Marketing
- Customer Experience
- AI
- Enterprise
- Video Generation
- Media
- Analytics
- Martech
---
