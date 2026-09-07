---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sci-corp.com
  spf: false
hosts:
- cert_expires: Nov 10 06:37:05 2026 GMT
  host: www.sci-corp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Service Corp International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Service Corp International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Service Corp International
provider_slug: service-corp-international
slug: service-corp-international-domain-security
source_filename: service-corp-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sci-corp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 06:37:05 2026 GMT\n  hsts: null\ndomains:\n- domain: sci-corp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnote: sci-corp.com publishes no MX, SPF, DMARC or CAA record and does not set HSTS; the absence of MX\n  means corporate mail is not delivered on this domain, so the SPF/DMARC gaps are a missing spoofing guard\n  on a web-only domain rather than a mail-authentication failure. TLS 1.3 is served. www.sci-corp.com\n  and the Dignity Memorial brand hosts sit behind a Cloudflare bot challenge that answers 403 to non-browser\n  clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-corp-international/refs/heads/main/security/service-corp-international-domain-security.yml
summary_line: TLSv1.3
tags:
- Fortune 1000
- Deathcare
- Funeral Services
- Cemeteries
- Cremation
- Consumer Services
---
