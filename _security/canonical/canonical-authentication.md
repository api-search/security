---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: canonical-snapd-rest-api-openapi.yml
  format: yaml
  label: snapd REST API
  slug: snapd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snapd-rest-api-openapi.yml
- filename: canonical-landscape-debarchive-api-openapi.yml
  format: yaml
  label: Landscape API
  slug: landscape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-landscape-debarchive-api-openapi.yml
- filename: canonical-assertions-api-openapi.yml
  format: yaml
  label: Canonical Assertions API
  slug: canonical-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-assertions-api-openapi.yml
- filename: canonical-search-api-openapi.yml
  format: yaml
  label: Canonical Search API
  slug: canonical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-search-api-openapi.yml
- filename: canonical-snaps-api-openapi.yml
  format: yaml
  label: Canonical Snaps API
  slug: canonical-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snaps-api-openapi.yml
- filename: canonical-lxd-rest-api-openapi.yml
  format: yaml
  label: LXD REST API
  slug: lxd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-lxd-rest-api-openapi.yml
- filename: canonical-ubuntu-security-api-openapi.json
  format: json
  label: Ubuntu Security API
  slug: ubuntu-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-ubuntu-security-api-openapi.json
- filename: canonical-pebble-api-openapi.yml
  format: yaml
  label: Pebble API
  slug: pebble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-pebble-api-openapi.yml
- filename: canonical-testflinger-api-openapi.json
  format: json
  label: Testflinger API
  slug: testflinger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-testflinger-api-openapi.json
- filename: canonical-hardware-api-openapi.json
  format: json
  label: Ubuntu Hardware API (hwapi)
  slug: hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-hardware-api-openapi.json
- filename: canonical-identity-platform-api-openapi.yml
  format: yaml
  label: Canonical Identity Platform API
  slug: identity-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-identity-platform-api-openapi.yml
- filename: canonical-test-observer-api-openapi.json
  format: json
  label: Test Observer API
  slug: test-observer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-test-observer-api-openapi.json
- filename: canonical-anbox-cloud-ams-api-openapi.json
  format: json
  label: Anbox Cloud AMS API
  slug: anbox-cloud-ams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-cloud-ams-api-openapi.json
- filename: canonical-anbox-stream-gateway-api-openapi.json
  format: json
  label: Anbox Stream Gateway API
  slug: anbox-stream-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-stream-gateway-api-openapi.json
- filename: canonical-cos-registration-server-api-openapi.yml
  format: yaml
  label: COS Registration Server API
  slug: cos-registration-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-cos-registration-server-api-openapi.yml
- filename: canonical-microceph-api-openapi.yml
  format: yaml
  label: MicroCeph REST API
  slug: microceph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-microceph-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Canonical Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Canonical secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Canonical
provider_slug: canonical
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://example.com/oauth/token
  name: OAuth2
  sources:
  - openapi/canonical-identity-platform-api-openapi.yml
  type: oauth2
- description: '**Unix Socket Peer Authentication**


    Authentication is not handled via traditional HTTP headers or tokens. Instead, it is managed at the operating system level using Unix domain socket peer credentials (e.g., `SO_PEERCRED` on Linux).


    **How It Works:**


    1.  The API server listens on a local Unix domain socket.

    2.  When a client connects to this socket, the server can ask the operating system kerne'
  in: header
  name: PeerAuth
  parameter: X-PEER-CREDENTIALS
  sources:
  - openapi/canonical-snapd-rest-api-openapi.yml
  type: apiKey
slug: canonical-authentication
source_filename: canonical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/canonical-identity-platform-api-openapi.yml, openapi/canonical-snapd-rest-api-openapi.yml;\n  upgraded 2026-09-05 by searching the Canonical product auth documentation and by live probing the API\n  hosts\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: There is no single Canonical credential. The derived scheme list below covers only the two specs\n    that declare securitySchemes; the portfolio actually uses five distinct models. The full picture is\n    in profiles[].\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/canonical-identity-platform-api-openapi.yml\n- name: PeerAuth\n  type: apiKey\n  in: header\n  parameter: X-PEER-CREDENTIALS\n  description: '**Unix Socket\
  \ Peer Authentication**\n\n\n    Authentication is not handled via traditional HTTP headers or tokens. Instead, it is managed at the\n    operating system level using Unix domain socket peer credentials (e.g., `SO_PEERCRED` on Linux).\n\n\n    **How It Works:**\n\n\n    1.  The API server listens on a local Unix domain socket.\n\n    2.  When a client connects to this socket, the server can ask the operating system kerne'\n  sources:\n  - openapi/canonical-snapd-rest-api-openapi.yml\ndocs:\n- https://documentation.ubuntu.com/lxd/latest/explanation/authentication/\n- https://snapcraft.io/docs/how-to-guides/snap-development/use-the-rest-api/\n- https://api.charmhub.io/docs/default.html\n- https://documentation.ubuntu.com/launchpad/user/how-to/launchpad-api/\nprofiles:\n- api: canonical:lxd-rest-api\n  primary: TLS client certificate\n  alternatives:\n  - OIDC bearer token\n  - unix socket group membership (local)\n  - bearer identity tokens\n  note: LXD trusts a client certificate added\
  \ to /1.0/certificates, or an OIDC identity under /1.0/auth/identities/oidc.\n    Local clients on the unix socket are authorized by group membership. Authorization is then resolved\n    through auth groups and permissions under /1.0/auth/groups.\n  evidence: openapi/canonical-lxd-rest-api-openapi.yml paths /1.0/certificates, /1.0/auth/identities/{tls,oidc,bearer},\n    /1.0/auth/groups\n- api: canonical:snapd-rest-api\n  primary: unix socket peer credentials (SO_PEERCRED)\n  note: Declared in the contract as the PeerAuth scheme. No HTTP token exists; reachability of /run/snapd.socket\n    with the right group membership IS the credential. Snaps get the restricted /run/snapd-snap.socket\n    instead.\n  evidence: openapi/canonical-snapd-rest-api-openapi.yml components.securitySchemes.PeerAuth\n- api: canonical:snap-store-api\n  primary: Ubuntu One macaroon\n  required_headers:\n  - Snap-Device-Series\n  note: The v2 device endpoints require a Snap-Device-Series header on every call, authenticated\
  \ or not.\n    Publisher operations against dashboard.snapcraft.io use a macaroon discharged by Ubuntu One SSO.\n  evidence: 'live probe 2026-09-05: GET https://api.snapcraft.io/v2/snaps/info/hello returned 400 with\n    {\"error-list\":[{\"code\":\"bad-argument\",\"message\":\"Snap-Device-Series header is required.\"}]}'\n- api: canonical:charmhub-api\n  primary: Charmhub developer token exchanged from an Ubuntu One macaroon\n  note: Macaroons issued by dashboard.snapcraft.io SSO are exchanged for a Charmhub developer token presented\n    in the Authorization header. Read endpoints such as /v2/charms/info/{name} are open.\n  evidence: 'live probe 2026-09-05: GET https://api.charmhub.io/v2/charms/info/postgresql-k8s returned\n    200 unauthenticated'\n- api: canonical:launchpad-api\n  primary: OAuth 1.0a\n  anonymous_access: read-only on public data\n  note: launchpadlib performs the OAuth 1.0a token exchange against login.launchpad.net. This is OAuth\n    1.0a, not 2.0.\n  evidence: https://documentation.ubuntu.com/launchpad/user/how-to/launchpad-api/\n\
  - api: canonical:ubuntu-security-api\n  primary: none\n  note: Fully open and unauthenticated.\n  evidence: 'live probe 2026-09-05: GET https://ubuntu.com/security/releases.json returned 200 with no\n    credential'\n- api: canonical:identity-platform-api\n  primary: OAuth 2.0 authorization code + OIDC\n  scopes:\n  - openid\n  - profile\n  - email\n  note: The authorizationUrl and tokenUrl in the published spec are https://example.com placeholders because\n    this is software a customer deploys; the real URLs are the deployment's own.\n  evidence: openapi/canonical-identity-platform-api-openapi.yml components.securitySchemes.OAuth2\ndiscovery:\n  openid_configuration: not served on any Canonical public host (16 hosts probed 2026-09-05, all 404)\n  oauth_authorization_server: not served on any Canonical public host (16 hosts probed 2026-09-05, all\n    404)\n  see: well-known/canonical-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/authentication/canonical-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Cloud
- Linux
- Open-Source
- Ubuntu
- Containers
- Bare Metal
- Charms
- Identity
---
