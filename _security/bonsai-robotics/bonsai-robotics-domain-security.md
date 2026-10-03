---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
- caa:
  - d1ibc16nuste3.cloudfront.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bonsairobotics.ai
  spf: true
hosts:
- cert_expires: Dec 21 07:53:45 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 16:51:45 2027 GMT
  host: bonsairobotics.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bonsai Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonsai Robotics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bonsai Robotics
provider_slug: bonsai-robotics
slug: bonsai-robotics-domain-security
source_filename: bonsai-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bonsairobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 16:51:45 2027 GMT\n  hsts: false\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bonsairobotics.ai\n  dnssec: true\n  caa:\n  - d1ibc16nuste3.cloudfront.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai-robotics/refs/heads/main/security/bonsai-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
