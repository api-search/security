---
description: ''
domains:
- caa:
  - 2e075f28e5244e838e548cba19e27540.vip1.huaweicloudwaf.com.
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ocft.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: ocft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oneconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OneConnect
provider_slug: oneconnect
slug: oneconnect-domain-security
source_filename: oneconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ocft.com\n  dnssec: false\n  caa:\n  - 2e075f28e5244e838e548cba19e27540.vip1.huaweicloudwaf.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneconnect/refs/heads/main/security/oneconnect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Financial Services
- Banking
- Insurance
- Artificial Intelligence
- Blockchain
- Cloud
- Technology as a Service
---
