---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_note: 'A syntactically valid DMARC policy (v=DMARC1; p=quarantine; pct=100; ruf=mailto:itsupport@fnality.org) is published as a TXT record on the APEX (fnality.com) instead of at _dmarc.fnality.com. RFC 7489 requires the record at the _dmarc subdomain, so `dig +short TXT _dmarc.fnality.com` returns nothing and receiving mail servers will not apply the policy. Recorded as dmarc: false because the policy is not discoverable where DMARC is looked up.'
  dnssec: false
  domain: fnality.com
  spf: true
hosts:
- cert_expires: Aug 18 09:03:03 2026 GMT
  host: fnality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.fnality.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Archbee-hosted documentation space (CNAME proxy.archbee.com). The space is credential-gated — the root returns HTTP 200 carrying a "Get a magic link to access space with your account" login shell rather than documentation.
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fnality International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fnality International, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fnality International
provider_slug: fnality-international
slug: fnality-international-domain-security
source_filename: fnality-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + the docs host (docs.fnality.com)\nhosts:\n- host: fnality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 09:03:03 2026 GMT\n  hsts: false\n- host: docs.fnality.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: cloudflare\n  note: >-\n    Archbee-hosted documentation space (CNAME proxy.archbee.com). The space is\n    credential-gated — the root returns HTTP 200 carrying a \"Get a magic link to\n    access space with your account\" login shell rather than documentation.\ndomains:\n- domain: fnality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_note: >-\n    A syntactically valid DMARC policy (v=DMARC1; p=quarantine; pct=100;\n    ruf=mailto:itsupport@fnality.org) is published as a TXT record on the APEX\n    (fnality.com) instead of at _dmarc.fnality.com. RFC 7489\
  \ requires the record\n    at the _dmarc subdomain, so `dig +short TXT _dmarc.fnality.com` returns\n    nothing and receiving mail servers will not apply the policy. Recorded as\n    dmarc: false because the policy is not discoverable where DMARC is looked up.\nx-observations:\n- host: fnality.com\n  finding: no HSTS on the primary website host\n- host: fnality.com\n  finding: >-\n    TLS certificate expiry observed as 2026-08-18, two days after this probe —\n    short-lived certificate rotation, not a defect, but noted as observed.\n- domain: fnality.com\n  finding: no CAA records published\n- domain: fnality.com\n  finding: DNSSEC not enabled\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnality-international/refs/heads/main/security/fnality-international-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Financial-Services
- Settlement
- Wholesale Banking
- Distributed Ledger
- Blockchain
- Financial Market Infrastructure
- Tokenisation
- Central Bank Money
- Liquidity Management
- Capital Markets
---
