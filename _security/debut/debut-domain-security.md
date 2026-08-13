---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: debutbiotech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deinde.com
  spf: true
hosts:
- cert_expires: Oct 14 17:07:37 2026 GMT
  host: www.debutbiotech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 20:50:03 2026 GMT
  host: www.deinde.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Debut, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Debut
provider_slug: debut
slug: debut-domain-security
source_filename: debut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.debutbiotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:07:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.deinde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:50:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: debutbiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: deinde.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debut/refs/heads/main/security/debut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Beauty
- Cosmetics
- Skincare
- Ingredients
- Synthetic Biology
- Artificial Intelligence
- Manufacturing
- Ecommerce
- Agentic Commerce
---
