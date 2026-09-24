---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ajaxhealth.com
  spf: true
hosts:
- cert_expires: Nov 12 00:05:19 2026 GMT
  host: ajaxhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ajaxhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ajaxhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ajaxhealth
provider_slug: ajaxhealth
slug: ajaxhealth-domain-security
source_filename: ajaxhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ajaxhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 00:05:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ajaxhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajaxhealth/refs/heads/main/security/ajaxhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Investment
- Healthcare
- MedTech
- VentureCapital
- Company
---
