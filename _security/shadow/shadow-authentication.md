---
api_key_in: []
auth_types:
- keystone-password
- keystone-application-credential
description: ''
kind: authentication
layout: security
method: searched
name: Shadow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shadow secures its APIs with keystone-password and keystone-application-credential across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shadow
provider_slug: shadow
scheme_count: 2
schemes:
- credential_delivery:
  - clouds.yaml (downloaded from the dashboard User Menu, "Get clouds.yaml file")
  - openrc.sh (shell environment file, same menu)
  description: Interactive and CLI authentication uses a domain-scoped username of the form user#domain (the docs give the example "user#mycompany-domain") plus a password, against the region's Keystone identity endpoint. The dashboard emits a ready-made clouds.yaml (Password Type) or openrc.sh which the operator saves to ~/.config/openstack/clouds.yaml and selects with the OS_CLOUD environment variable.
  name: Keystone password (domain-scoped user)
  protocol: OpenStack Identity API v3
  recommended_for: interactive / human operators
  source: https://gpu-instances.shadow.tech/docs/cli-guide/configuration/
  type: password
- description: The documented mechanism for authenticating applications and scripts without sharing the primary account password. Created in the dashboard User Center under "Application Credentials" with a name, an optional expiration date, and a selected set of roles. Shadow's docs state the benefits verbatim as limited scope (restricted to specific projects), fine-grained access control (exact roles and permissions), easy revocation (deleted without affecting the main account), reduced risk (a compromise affects only that credential), and auditing (easier to track which application or script is making specific API calls).
  name: Keystone Application Credential
  protocol: OpenStack Identity API v3
  recommended_for: automation, third-party applications, scripts, CI/CD
  revocation: Delete Application Credential from the Application Credentials page
  rotation_guidance: 'Documented best practice: "Regularly audit and rotate your application credentials."'
  source: https://gpu-instances.shadow.tech/docs/getting-started/security-measures/
  type: application-credential
slug: shadow-authentication
source_filename: shadow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://gpu-instances.shadow.tech/docs/getting-started/security-measures/\ndocs:\n- https://gpu-instances.shadow.tech/docs/getting-started/security-measures/\n- https://gpu-instances.shadow.tech/docs/cli-guide/configuration/\n- https://gpu-instances.shadow.tech/docs/getting-started/skyline-interface/\n- https://gpu-instances.shadow.tech/docs/getting-started/project-management/\nnote: >-\n  Shadow publishes no OpenAPI document, so this profile could not be derived mechanically. It was\n  read from Shadow GPU's own documentation and confirmed against a live anonymous probe of the\n  Keystone identity endpoint. Shadow GPU is a curated OpenStack 2024.1 deployment, so its\n  authentication model IS the OpenStack Keystone v3 model — there is no Shadow-specific token\n  scheme, API-key header, or OAuth 2.0 authorization server.\nsummary:\n  types:\n  - keystone-password\n  - keystone-application-credential\n  api_key_in: []\n  oauth2_flows:\
  \ []\n  standard: OpenStack Identity API v3 (Keystone)\n  identity_api_version: v3.14\n  probed_anonymously: true\nschemes:\n- name: Keystone password (domain-scoped user)\n  type: password\n  protocol: OpenStack Identity API v3\n  description: >-\n    Interactive and CLI authentication uses a domain-scoped username of the form user#domain (the\n    docs give the example \"user#mycompany-domain\") plus a password, against the region's Keystone\n    identity endpoint. The dashboard emits a ready-made clouds.yaml (Password Type) or openrc.sh\n    which the operator saves to ~/.config/openstack/clouds.yaml and selects with the OS_CLOUD\n    environment variable.\n  credential_delivery:\n  - clouds.yaml (downloaded from the dashboard User Menu, \"Get clouds.yaml file\")\n  - openrc.sh (shell environment file, same menu)\n  source: https://gpu-instances.shadow.tech/docs/cli-guide/configuration/\n  recommended_for: interactive / human operators\n- name: Keystone Application Credential\n  type:\
  \ application-credential\n  protocol: OpenStack Identity API v3\n  description: >-\n    The documented mechanism for authenticating applications and scripts without sharing the\n    primary account password. Created in the dashboard User Center under \"Application Credentials\"\n    with a name, an optional expiration date, and a selected set of roles. Shadow's docs state the\n    benefits verbatim as limited scope (restricted to specific projects), fine-grained access\n    control (exact roles and permissions), easy revocation (deleted without affecting the main\n    account), reduced risk (a compromise affects only that credential), and auditing (easier to\n    track which application or script is making specific API calls).\n  rotation_guidance: 'Documented best practice: \"Regularly audit and rotate your application credentials.\"'\n  revocation: Delete Application Credential from the Application Credentials page\n  source: https://gpu-instances.shadow.tech/docs/getting-started/security-measures/\n\
  \  recommended_for: automation, third-party applications, scripts, CI/CD\nidentity_endpoints:\n  note: >-\n    Probed anonymously on 2026-08-17. Shadow's published \"Regions and Endpoints\" page lists only the\n    portal (dashboard) URLs; the Keystone identity endpoints below were discovered by probe and are\n    self-attested by the API — the version document returns its own href, e.g.\n    https://auth.uswdc01.os.shadow.tech/v3/ — which is what proves the host belongs to Shadow. The\n    remainder of the OpenStack service catalog (Nova, Neutron, Cinder, Glance, Octavia, Designate,\n    Barbican, Placement, CloudKitty) is returned only inside an authenticated token response and is\n    therefore not publicly enumerable.\n  version_document_media_type: application/vnd.openstack.identity-v3+json\n  endpoints:\n  - region: FRSBG01\n    location: Strasbourg, France\n    url: https://auth.frsbg01.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: 'FAIL — certificate\
  \ expired Jul 1 08:49:57 2026 GMT (CN=api.frsbg01.os.shadow.tech); a\n      strict-TLS client cannot complete a handshake against this identity endpoint'\n  - region: FRSBG02\n    location: Strasbourg, France (Edge)\n    url: https://auth.frsbg02.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Oct 13 10:52:22 2026 GMT\n  - region: FRDUN02\n    location: Dunkirk, France\n    url: https://auth.frdun02.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Nov  6 02:15:42 2026 GMT\n  - region: DEFRA01\n    location: Frankfurt, Germany\n    url: https://auth.defra01.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Nov 15 06:59:02 2026 GMT\n  - region: USWDC01\n    location: Washington DC, USA\n    url: https://auth.uswdc01.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Oct  1 08:55:45 2026 GMT\n  - region: USPOR01\n    location: Portland,\
  \ USA\n    url: https://auth.uspor01.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Sep  9 08:08:52 2026 GMT\n  - region: CAMTL01\n    location: Montreal, Canada\n    url: https://auth.camtl01.os.shadow.tech/v3\n    http_status: 200\n    identity_version: v3.14\n    tls: valid to Sep 22 11:09:08 2026 GMT\nauthorization:\n  model: Keystone role-based access control, project-scoped\n  note: >-\n    Shadow GPU has no OAuth 2.0 scope surface; authorization is expressed as Keystone role\n    assignments on a project. Roles below are quoted from Shadow's own documentation with the\n    Keystone role names it publishes.\n  roles:\n  - label: Member\n    keystone_role: member\n    description: Access to all project services, but cannot invite others or modify roles.\n  - label: Project Moderator\n    keystone_role: project_mod\n    description: Can invite users and update their roles, but cannot change the project admin.\n  - label: Project Administrator\n\
  \    keystone_role: project_admin\n    description: Complete management of the project, including user invitations and role assignments.\n  - label: Load Balancer Reader\n    keystone_role: load-balancer_observer\n    description: Can view load balancers and their configurations.\n  - label: Load Balancer Member\n    keystone_role: load-balancer_member\n    description: Can manage load balancers and their configurations.\n  - label: Secret Creator\n    keystone_role: creator\n    description: Can create and manage secrets.\n  - label: Secret Reader\n    keystone_role: observer\n    description: Can view secrets.\n  verify_command: openstack role assignment list --user <your-user-id> --project <your-project-id>\n  source: https://gpu-instances.shadow.tech/docs/getting-started/project-management/\nuser_provisioning:\n  service: Adjutant (OpenStack project-user invitation workflow)\n  cli: openstack project user invite <email-address> <role-name>\n  list: openstack project user list\n  note:\
  \ >-\n    Invitations are completed by the invitee through the dashboard (choose an initial password). An\n    advanced CLI-only path exists for automation via Adjutant's admin task interface\n    (openstack admin task token submit <invitation-token> '{\"password\": \"...\"}'). Requires\n    project_mod or project_admin.\n  source: https://gpu-instances.shadow.tech/docs/cli-guide/user-management/\nnot_found:\n  - 'no OAuth 2.0 / OpenID Connect authorization server: /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return 404 on shadow.tech and an HTML SPA shell (soft\n    200) on gpu-instances.shadow.tech'\n  - 'no API-key scheme documented for Shadow GPU'\n  - 'no mutual TLS / client-certificate option documented'\n  - 'no published OpenAPI securitySchemes to derive from'\n  - 'no self-service password reset: \"Contact your OpenStack administrator through the established\n    support channels. For security reasons, password resets require verification\
  \ of your identity and\n    cannot be performed through self-service.\" (docs FAQ)'\nx-evidence:\n  fetched: '2026-08-17'\n  probes:\n  - url: https://auth.uswdc01.os.shadow.tech/v3\n    status: 200\n    finding: Keystone v3.14 version document, self-href https://auth.uswdc01.os.shadow.tech/v3/\n  - url: https://auth.frsbg01.os.shadow.tech/v3\n    status: 200\n    finding: same version document, but TLS certificate expired 2026-07-01\n  - url: https://shadow.tech/.well-known/openid-configuration\n    status: 404\n  - url: https://developers.shadow.tech/\n    status: 403\n    finding: legacy developer portal now redirects to support.shadow.tech/hc/en-us\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadow/refs/heads/main/authentication/shadow-authentication.yml
summary_line: keystone-password/keystone-application-credential · 2 schemes
tags:
- Company
- Cloud Computing
- GPU
- Cloud Gaming
- Infrastructure
- OpenStack
- AI Infrastructure
- Compute
- Storage
- Europe
---
