---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thepollyproject.org
  spf: false
hosts:
- cert_expires: Oct  6 18:54:30 2026 GMT
  host: www.thepollyproject.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Polly
provider_slug: polly
slug: polly-domain-security
source_filename: polly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thepollyproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:54:30 2026 GMT\n  hsts: false\ndomains:\n- domain: thepollyproject.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polly/refs/heads/main/security/polly-domain-security.yml
summary_line: TLSv1.3
tags:
- .NET
- C#
- Circuit Breaker
- Fault Tolerance
- Microservices
- Rate Limiter
- Resilience
- Retry
- Timeout
---
