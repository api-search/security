---
api_specs:
- filename: obeliskgate-com-account-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Account API
  slug: obeliskgate-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-account-api-openapi.yml
- filename: obeliskgate-com-agent-identity-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Agent Identity API
  slug: obeliskgate-com-agent-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-agent-identity-api-openapi.yml
- filename: obeliskgate-com-app-registration-api-openapi.yml
  format: yaml
  label: VaultSpark Studios App Registration API
  slug: obeliskgate-com-app-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-app-registration-api-openapi.yml
- filename: obeliskgate-com-auth-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Auth API
  slug: obeliskgate-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-auth-api-openapi.yml
- filename: obeliskgate-com-contact-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Contact API
  slug: obeliskgate-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-contact-api-openapi.yml
- filename: obeliskgate-com-email-verification-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Email Verification API
  slug: obeliskgate-com-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-email-verification-api-openapi.yml
- filename: obeliskgate-com-fedcm-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Fedcm API
  slug: obeliskgate-com-fedcm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-fedcm-api-openapi.yml
- filename: obeliskgate-com-federation-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Federation API
  slug: obeliskgate-com-federation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-federation-api-openapi.yml
- filename: obeliskgate-com-mcp-api-openapi.yml
  format: yaml
  label: VaultSpark Studios MCP API
  slug: obeliskgate-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-mcp-api-openapi.yml
- filename: obeliskgate-com-organizations-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Organizations API
  slug: obeliskgate-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-organizations-api-openapi.yml
- filename: obeliskgate-com-project-profile-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Project Profile API
  slug: obeliskgate-com-project-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-project-profile-api-openapi.yml
- filename: obeliskgate-com-proof-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Proof API
  slug: obeliskgate-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-proof-api-openapi.yml
- filename: obeliskgate-com-release-history-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Release History API
  slug: obeliskgate-com-release-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-release-history-api-openapi.yml
- filename: obeliskgate-com-scan-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Scan API
  slug: obeliskgate-com-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-scan-api-openapi.yml
- filename: obeliskgate-com-seal-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Seal API
  slug: obeliskgate-com-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-seal-api-openapi.yml
- filename: obeliskgate-com-studio-ecosystem-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Studio Ecosystem API
  slug: obeliskgate-com-studio-ecosystem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-studio-ecosystem-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: obeliskgate.com
  spf: true
hosts:
- cert_expires: Jan  1 22:04:29 2027 GMT
  host: obeliskgate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: VaultSpark Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VaultSpark Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VaultSpark Studios
provider_slug: obeliskgate-com
slug: obeliskgate-com-domain-security
source_filename: obeliskgate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obeliskgate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:04:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: obeliskgate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/obeliskgate-com/security/obeliskgate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Security
- Identity
- Passkeys
- Artificial Intelligence
---
