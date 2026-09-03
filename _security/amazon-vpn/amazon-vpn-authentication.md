---
api_key_in:
- header
api_specs:
- filename: amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api-openapi.yml
  format: yaml
  label: Amazon VPN AWS VPN API (Amazon EC2 Query API Subset) API
  slug: amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-vpn/refs/heads/main/openapi/amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Amazon Vpn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon VPN secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon VPN
provider_slug: amazon-vpn
scheme_count: 1
schemes:
- algorithm: AWS4-HMAC-SHA256
  credential_scope: <date>/<region>/ec2/aws4_request
  description: AWS Signature Version 4 signed request.
  in: header
  name: SigV4
  optional_headers:
  - X-Amz-Security-Token
  parameter: Authorization
  required_headers:
  - Authorization
  - X-Amz-Date
  - Host
  sources:
  - openapi/amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api-openapi.yml
  type: apiKey
slug: amazon-vpn-authentication
source_filename: amazon-vpn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://docs.aws.amazon.com/AWSEC2/latest/APIReference/Query-Requests.html\ndocs:\n  - https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_sigv.html\n  - https://docs.aws.amazon.com/AWSEC2/latest/APIReference/CommonParameters.html\n  - https://docs.aws.amazon.com/vpn/latest/s2svpn/security-iam.html\n  - https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonec2.html\nderived_from: openapi/amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    The OpenAPI models SigV4 as `apiKey in header Authorization`, which is the closest\n    OpenAPI 3.x can express. It is not a static API key: the Authorization header carries\n    an AWS4-HMAC-SHA256 signature computed per request over a canonical request, a\n    credential scope (date/region/service) and a derived\
  \ signing key.\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  algorithm: AWS4-HMAC-SHA256\n  description: AWS Signature Version 4 signed request.\n  credential_scope: <date>/<region>/ec2/aws4_request\n  required_headers: [Authorization, X-Amz-Date, Host]\n  optional_headers: [X-Amz-Security-Token]\n  sources:\n  - openapi/amazon-vpn-aws-vpn-api-amazon-ec2-query-api-subset-api-openapi.yml\ncredential_types:\n  - kind: long-lived-access-key\n    identifier_prefix: AKIA\n    note: IAM user access key ID and secret. AWS discourages these in favour of roles.\n  - kind: temporary-credentials\n    identifier_prefix: ASIA\n    extra_header: X-Amz-Security-Token\n    note: STS session credentials from an assumed role or IAM Identity Center. Expire; ExpiredTokenException on reuse.\nauthorization:\n  model: aws-iam-policy\n  scopes: false\n  scopes_note: >-\n    There is no OAuth scope surface on this API — which is why scopes/ is absent from\n    this repo\
  \ rather than empty. Authorization is IAM policy evaluated per request\n    against action-level permissions.\n  permission_namespace: 'ec2:'\n  permissions_reference: https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonec2.html\n  vpn_permissions:\n    - ec2:CreateVpnConnection\n    - ec2:DescribeVpnConnections\n    - ec2:DeleteVpnConnection\n    - ec2:ModifyVpnConnection\n    - ec2:ModifyVpnConnectionOptions\n    - ec2:ModifyVpnTunnelCertificate\n    - ec2:ModifyVpnTunnelOptions\n    - ec2:CreateVpnConnectionRoute\n    - ec2:DeleteVpnConnectionRoute\n    - ec2:CreateCustomerGateway\n    - ec2:DescribeCustomerGateways\n    - ec2:DeleteCustomerGateway\n    - ec2:CreateVpnGateway\n    - ec2:DescribeVpnGateways\n    - ec2:DeleteVpnGateway\n    - ec2:AttachVpnGateway\n    - ec2:DetachVpnGateway\n    - ec2:EnableVgwRoutePropagation\n    - ec2:DisableVgwRoutePropagation\n    - ec2:CreateClientVpnEndpoint\n    - ec2:DescribeClientVpnEndpoints\n    - ec2:DeleteClientVpnEndpoint\n\
  \    - ec2:ModifyClientVpnEndpoint\n    - ec2:AssociateClientVpnTargetNetwork\n    - ec2:DisassociateClientVpnTargetNetwork\n    - ec2:AuthorizeClientVpnIngress\n    - ec2:RevokeClientVpnIngress\n    - ec2:ImportClientVpnClientCertificateRevocationList\n    - ec2:ExportClientVpnClientCertificateRevocationList\n    - ec2:CreateClientVpnRoute\n    - ec2:DeleteClientVpnRoute\n    - ec2:DescribeClientVpnConnections\n    - ec2:TerminateClientVpnConnections\n  service_linked_role: AWSServiceRoleForVPCS2SVPN\n  managed_policy: AWSVPCS2SVpnServiceRolePolicy\n  managed_policy_docs: https://docs.aws.amazon.com/vpn/latest/s2svpn/s2s-security-iam-awsmanpol.html\npermission_check:\n  parameter: DryRun\n  success_error: DryRunOperation\n  failure_error: UnauthorizedOperation\n  note: The API ships a first-class way to test authorization without acting. See conventions/amazon-vpn-conventions.yml.\nauth_failures:\n  - code: AuthFailure\n    status: 401\n    cause: Unsigned request. Observed live on 2026-09-01\
  \ across every /.well-known/ probe of ec2.amazonaws.com.\n  - code: IncompleteSignature\n    status: 400\n    cause: Malformed SigV4 signature.\n  - code: MissingAuthenticationToken\n    status: 403\n    cause: No credentials presented.\n  - code: ExpiredTokenException\n    status: 403\n    cause: STS session credentials expired.\n  - code: UnrecognizedClientException\n    status: 403\n    cause: Access key ID not recognised.\n  - code: AccessDeniedException\n    status: 403\n    cause: Credentials valid, IAM policy does not permit the action.\ntunnel_authentication:\n  note: >-\n    Distinct from API authentication — this is how the VPN tunnel itself authenticates,\n    and it is a separate concern an agent must not conflate with the API credential.\n  options:\n    - kind: pre-shared-key\n      default: true\n      storage: [site-to-site-vpn-service, aws-secrets-manager]\n      secrets_manager_since: '2025-05-27'\n    - kind: private-certificate\n      authority: AWS Private Certificate\
  \ Authority\n      docs: https://docs.aws.amazon.com/vpn/latest/s2svpn/vpn-tunnel-authentication-options.html\n    - kind: client-vpn-mutual-authentication\n      scope: AWS Client VPN\n      note: X.509 server and client certificates in AWS Certificate Manager, generated with OpenVPN easy-rsa.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpn/refs/heads/main/authentication/amazon-vpn-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- Security
- VPN
- IPsec
- Hybrid Cloud
- Connectivity
- Infrastructure
---
