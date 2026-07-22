---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: latenthealth.com
  spf: true
hosts:
- cert_expires: Sep 15 06:36:03 2026 GMT
  host: latenthealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Latent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Latent
provider_slug: latent
slug: latent-domain-security
source_filename: latent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latenthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:36:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: latenthealth.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latent/refs/heads/main/security/latent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Systems
- Pharmacy
- Prior Authorization
- Medication Access
- Clinical AI
- 340B
- EHR Integration
- Artificial Intelligence
---
