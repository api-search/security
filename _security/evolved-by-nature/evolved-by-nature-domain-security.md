---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evolvedbynature.com
  spf: true
hosts:
- cert_expires: Sep 29 14:17:40 2026 GMT
  host: biotech.evolvedbynature.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 10:35:02 2026 GMT
  host: skincare.evolvedbynature.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:50:01 2026 GMT
  host: bioactives.evolvedbynature.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolved By Nature Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evolved By Nature, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evolved By Nature
provider_slug: evolved-by-nature
slug: evolved-by-nature-domain-security
source_filename: evolved-by-nature-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biotech.evolvedbynature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:17:40 2026 GMT\n  hsts: false\n- host: skincare.evolvedbynature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: bioactives.evolvedbynature.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:50:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: evolvedbynature.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolved-by-nature/refs/heads/main/security/evolved-by-nature-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Materials Science
- Sustainability
- Personal Care
- Cosmetics
- Specialty Chemicals
- Textiles
- eCommerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
---
