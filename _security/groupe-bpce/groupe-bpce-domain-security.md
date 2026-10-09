---
api_specs:
- filename: groupe-bpce-aisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE AISP API
  slug: groupe-bpce-aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-aisp-api-openapi.yml
- filename: groupe-bpce-cbpii-api-openapi.yml
  format: yaml
  label: Groupe BPCE CBPII API
  slug: groupe-bpce-cbpii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-cbpii-api-openapi.yml
- filename: groupe-bpce-external-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE External Accounts API
  slug: groupe-bpce-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-external-accounts-api-openapi.yml
- filename: groupe-bpce-internal-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE Internal Accounts API
  slug: groupe-bpce-internal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-internal-accounts-api-openapi.yml
- filename: groupe-bpce-pisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE PISP API
  slug: groupe-bpce-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-pisp-api-openapi.yml
- filename: groupe-bpce-registration-api-openapi.yml
  format: yaml
  label: Groupe BPCE Registration API
  slug: groupe-bpce-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-registration-api-openapi.yml
- filename: groupe-bpce-transfers-api-openapi.yml
  format: yaml
  label: Groupe BPCE Transfers API
  slug: groupe-bpce-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-transfers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuevmc "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: groupebpce.com
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: groupebpce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Groupe Bpce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groupe BPCE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Groupe BPCE
provider_slug: groupe-bpce
slug: groupe-bpce-domain-security
source_filename: groupe-bpce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groupebpce.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: groupebpce.com\n  dnssec: false\n  caa:\n  - 0 issuevmc \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/security/groupe-bpce-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Banking
- Financial Services
- Open Banking
- PSD2
- Payments
- Insurance
- France
---
