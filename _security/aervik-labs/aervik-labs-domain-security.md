---
api_specs:
- filename: aervik-labs-parse-api-openapi.yml
  format: yaml
  label: Aervik Labs Parse API
  slug: aervik-labs-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-parse-api-openapi.yml
- filename: aervik-labs-requirements-api-openapi.yml
  format: yaml
  label: Aervik Labs Requirements API
  slug: aervik-labs-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-requirements-api-openapi.yml
- filename: aervik-labs-verify-api-openapi.yml
  format: yaml
  label: Aervik Labs Verify API
  slug: aervik-labs-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aerviklabs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Nov 25 11:39:46 2026 GMT
  host: aerviklabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: certificate-of-insurance-verification-compliance-check-api.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aervik Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aervik Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aervik Labs
provider_slug: aervik-labs
slug: aervik-labs-domain-security
source_filename: aervik-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aerviklabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 11:39:46 2026 GMT\n  hsts: false\n- host: certificate-of-insurance-verification-compliance-check-api.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aerviklabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/security/aervik-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Compliance
- Verification
- Insurtech
- Certificate of Insurance
- ACORD 25
- Document Intelligence
- RapidAPI
---
