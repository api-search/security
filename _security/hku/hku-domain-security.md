---
api_specs:
- filename: hku-identity-openapi.yml
  format: yaml
  label: HKU AD FS OAuth 2.0 / OpenID Connect Issuer
  slug: adfs-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-identity-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "hongkongpost.gov.hk"
  - 0 issue "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hku.hk
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hkaf.edu.hk
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.hku.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.hkaf.edu.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: hkafidp.hku.hk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Hong Kong, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Hong Kong
provider_slug: hku
slug: hku-domain-security
source_filename: hku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hku.hk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hkaf.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: hkafidp.hku.hk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hku.hk\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"hongkongpost.gov.hk\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hkaf.edu.hk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/security/hku-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Hong Kong
- Identity Federation
- Single Sign-On
- Research Data
- Open Access
- Artificial Intelligence
- Research Computing
---
