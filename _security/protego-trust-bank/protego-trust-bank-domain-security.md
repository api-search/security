---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: protegotrust.com
  spf: true
hosts:
- host: www.protegotrust.com
  https: false
kind: domain-security
layout: security
method: probed
name: Protego Trust Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protego Trust Bank, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Protego Trust Bank
provider_slug: protego-trust-bank
slug: protego-trust-bank-domain-security
source_filename: protego-trust-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.protegotrust.com\n  https: false\ndomains:\n- domain: protegotrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes: >-\n  Both www.protegotrust.com and protegotrust.com terminate the TLS handshake with a fatal\n  internal_error alert (SSL alert 80) and present no certificate, so https is recorded as\n  false for transport failure rather than for a missing redirect. Plain HTTP 301-redirects\n  to the same unreachable HTTPS origin. Reproduced 2026-08-26 from curl/LibreSSL, OpenSSL\n  s_client, and a headless-Chromium fetch (ERR_SSL_PROTOCOL_ERROR). The hosts are Webflow\n  proxy endpoints (proxy-ssl.webflow.com) whose custom-domain certificate is not\n  provisioned. No CAA record is published; DNSSEC is signed and SPF/DMARC are present, so\n  the zone is actively administered while the web front end is dark.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protego-trust-bank/refs/heads/main/security/protego-trust-bank-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Banking
- Financial Services
- Digital Assets
- Cryptocurrency
- Custody
- Trust Bank
- Institutional
- United States
---
