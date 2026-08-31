---
api_key_in: []
api_specs:
- filename: metalenz-press-releases-api-openapi.yml
  format: yaml
  label: Metalenz Press Releases API
  slug: metalenz-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-press-releases-api-openapi.yml
- filename: metalenz-pages-api-openapi.yml
  format: yaml
  label: Metalenz Pages API
  slug: metalenz-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-pages-api-openapi.yml
- filename: metalenz-media-api-openapi.yml
  format: yaml
  label: Metalenz Media API
  slug: metalenz-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-media-api-openapi.yml
- filename: metalenz-taxonomy-api-openapi.yml
  format: yaml
  label: Metalenz Taxonomy API
  slug: metalenz-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-taxonomy-api-openapi.yml
- filename: metalenz-search-api-openapi.yml
  format: yaml
  label: Metalenz Search API
  slug: metalenz-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-search-api-openapi.yml
- filename: metalenz-discovery-api-openapi.yml
  format: yaml
  label: Metalenz Discovery API
  slug: metalenz-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-discovery-api-openapi.yml
- filename: metalenz-oembed-api-openapi.yml
  format: yaml
  label: Metalenz oEmbed API
  slug: metalenz-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-oembed-api-openapi.yml
auth_types: []
description: Metalenz publishes no developer program and issues no API credentials. The WordPress REST content API behind metalenz.com is anonymously readable — no key, token, signature or account is required to read press releases, pages, media, taxonomies, search, oEmbed or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface. Separately, Metalenz runs a credential-gated documentation portal at docs.metalenz.com behind Microsoft Entra ID; that is a human login, not an API credential.
kind: authentication
layout: security
method: probed
name: Metalenz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metalenz declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Metalenz
provider_slug: metalenz
scheme_count: 0
schemes: []
slug: metalenz-authentication
source_filename: metalenz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://metalenz.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  Metalenz publishes no developer program and issues no API credentials. The WordPress REST content\n  API behind metalenz.com is anonymously readable — no key, token, signature or account is required\n  to read press releases, pages, media, taxonomies, search, oEmbed or the discovery metadata. The\n  server declares exactly one authentication method in its own root document, WordPress application\n  passwords, and that method gates only the write and privileged-read operations that are not part\n  of the public surface. Separately, Metalenz runs a credential-gated documentation portal at\n  docs.metalenz.com behind Microsoft Entra ID; that is a human login, not an API credential.\nsummary:\n  types: []\n  anonymous_read: true\n  credentialed_write: true\n  api_key_in: []\n  oauth2_flows: []\n  note:\
  \ >-\n    No securityScheme appears in any of the seven derived OpenAPI documents because the public\n    surface genuinely has none. This is a recorded absence, not a gap in harvesting.\nschemes: []\ndeclared_by_server:\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords (RFC 7617 Basic over TLS, username + generated application\n    password). Declared in the `authentication` block of the API root document. Required for every\n    write method and for privileged reads such as GET /wp/v2/settings, /wp/v2/themes,\n    /wp/v2/plugins, /wp/v2/menus and the whole widget/template/global-styles surface. Credentials\n    are issued per WordPress user from the site admin — there is no public registration path, so\n    this is a staff-only credential, not a developer credential.\n  authorization_endpoint: https://metalenz.com/wp-admin/authorize-application.php\n  source: https://metalenz.com/wp-json/\nadjacent_identity_systems:\n\
  - name: Microsoft Entra ID (Azure AD)\n  applies_to: https://docs.metalenz.com/documentation/\n  protocol: OpenID Connect 1.0 (implicit id_token, prompt=select_account)\n  tenant: 8dd6aaa4-ef1b-4a81-a14f-ef61ccec4361\n  issuer: https://login.microsoftonline.com/8dd6aaa4-ef1b-4a81-a14f-ef61ccec4361/v2.0\n  authorization_endpoint: https://login.microsoftonline.com/8dd6aaa4-ef1b-4a81-a14f-ef61ccec4361/oauth2/v2.0/authorize\n  scopes_supported: [openid, profile, email, offline_access]\n  detail: >-\n    docs.metalenz.com serves a two-line landing page linking to /documentation/, which 301s to\n    /documentation/ and then redirects into the Microsoft Entra ID authorize endpoint for the\n    Metalenz tenant. This is Metalenz's customer/partner documentation for its optics products and\n    it is not reachable without an account. It is recorded here because it is the only identity\n    surface Metalenz operates, but it protects human documentation, not an API: no API is\n    advertised behind\
  \ it and no protected-resource metadata is published. The tenant and client\n    identifiers above are public values emitted in the redirect URL, not secrets.\nevidence:\n- url: https://metalenz.com/wp-json/\n  http_status: 200\n  finding: 'authentication: {\"application-passwords\": {\"endpoints\": {\"authorization\": \"https://metalenz.com/wp-admin/authorize-application.php\"}}}'\n- url: https://metalenz.com/wp-json/wp/v2/posts?per_page=2\n  http_status: 200\n  finding: 'Anonymous read succeeds; response carries `Allow: GET`, confirming read-only anonymous access. X-WP-Total 26.'\n- url: https://metalenz.com/wp-json/wp/v2/media?per_page=2\n  http_status: 200\n  finding: Anonymous read of the media library succeeds, X-WP-Total 418.\n- url: https://metalenz.com/wp-json/wp/v2/settings\n  http_status: 401\n  finding: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n- url: https://metalenz.com/wp-json/wp/v2/themes\n  http_status:\
  \ 401\n  finding: 'Privileged read is credential-gated: {\"code\":\"rest_cannot_view_themes\",...}'\n- url: https://docs.metalenz.com/documentation\n  http_status: 301\n  finding: 301 to /documentation/, which redirects into login.microsoftonline.com — Entra ID gate.\n- url: https://login.microsoftonline.com/8dd6aaa4-ef1b-4a81-a14f-ef61ccec4361/v2.0/.well-known/openid-configuration\n  http_status: 200\n  finding: OpenID Provider metadata for the Metalenz tenant; confirms the gate is OIDC.\nx-evidence:\n  fetched: '2026-08-25'\n  probes: 7\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/authentication/metalenz-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Semiconductors
- Optics
- Meta-Optics
- Metasurface
- Photonics
- Biometrics
- Face Authentication
- Polarization Imaging
- 3D Sensing
- Computer-Vision
- Consumer Electronics
- Automotive
- Robotics
- Hardware
- Content
---
