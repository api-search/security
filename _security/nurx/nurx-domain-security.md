---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nurx.co
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: app.nurx.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nurx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nurx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nurx
provider_slug: nurx
slug: nurx-domain-security
source_filename: nurx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.nurx.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nurx.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nurx/refs/heads/main/security/nurx-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Health
- Telehealth
- Pharmacy
- Women's Health
- Reproductive Health
- Prescriptions
---
