---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: biohmhealth.com
  spf: true
hosts:
- cert_expires: Dec 24 01:40:33 2026 GMT
  host: www.biohmhealth.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biohmhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biohmhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Biohmhealth
provider_slug: biohmhealth
slug: biohmhealth-domain-security
source_filename: biohmhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biohmhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 01:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: biohmhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biohmhealth/refs/heads/main/security/biohmhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Probiotics
- Supplements
- Gut Health
- E-Commerce
---
