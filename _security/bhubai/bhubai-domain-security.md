---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bhubai.com
  spf: true
hosts:
- cert_expires: Dec 29 06:17:18 2026 GMT
  host: bhubai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bhubai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bhubai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bhubai
provider_slug: bhubai
slug: bhubai-domain-security
source_filename: bhubai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bhubai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 06:17:18 2026 GMT\n  hsts: false\ndomains:\n- domain: bhubai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bhubai/refs/heads/main/security/bhubai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API
- Technology
- Platform
- Services
---
