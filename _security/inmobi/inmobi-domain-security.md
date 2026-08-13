---
description: ''
domains:
- caa: []
  caa_note: No CAA record — any public CA may issue for inmobi.com.
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: dmarc-report@inmobi.com
  dmarc_ruf: dmarc-report@inmobi.com
  dmarc_subdomain_policy: quarantine
  dnssec: false
  domain: inmobi.com
  spf: true
  spf_policy: -all (hard fail)
  spf_record: v=spf1 ip4:50.213.20.161 ip4:209.214.228.18 ip4:101.254.125.194 ip4:123.127.0.146 include:_s00230767.autospf.email include:outbound.mailhop.org include:2714195.spf01.hubspotemail.net -all
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.inmobi.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header on the primary brand host.
  role: corporate site
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: support.inmobi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: documentation
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.inmobi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: The root path 302-redirects to a blackhole and returns no HSTS; the header is present on the routed API path /v3.0/reporting/publisher.
  other_headers:
    x-content-type-options: nosniff
    x-dns-prefetch-control: 'off'
    x-download-options: noopen
    x-frame-options: SAMEORIGIN
    x-xss-protection: 1; mode=block
  role: Publisher Reporting API
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: publisher.inmobi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  role: Ad Management API + publisher dashboard
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.cdr.inmobi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: DSP Cost API
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.w.inmobi.com
  hsts: false
  https: true
  role: Server-to-Server Ad Request API
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: advertising.inmobi.com
  hsts: false
  https: true
  role: advertiser marketing site
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inmobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InMobi, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InMobi
provider_slug: inmobi
slug: inmobi-domain-security
source_filename: inmobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every host named in apis.yml, 2026-08-12\n  (probe-domain-security.py output extended by hand to cover the three API hosts\n  the script does not read: publisher.inmobi.com, api.cdr.inmobi.com and\n  api.w.inmobi.com)\nnotes: >-\n  The finding worth carrying forward: InMobi's API hosts are hardened but its\n  PUBLIC-FACING hosts are not. api.inmobi.com, publisher.inmobi.com and\n  api.cdr.inmobi.com all return Strict-Transport-Security with includeSubDomains\n  on their API paths, while www.inmobi.com — the host the brand, the Trust\n  Center and every policy document live on — serves no HSTS header at all. The\n  domain has no DNSSEC and no CAA record, so certificate issuance for\n  inmobi.com is unconstrained. Email authentication is the strongest part of the\n  posture: SPF ends in a hard fail and DMARC is at p=quarantine with 100%\n  coverage, aggregate and forensic reporting, and an explicit\
  \ subdomain policy.\nhosts:\n- host: www.inmobi.com\n  role: corporate site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: false\n  note: No Strict-Transport-Security header on the primary brand host.\n- host: support.inmobi.com\n  role: documentation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inmobi.com\n  role: Publisher Reporting API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: >-\n    The root path 302-redirects to a blackhole and returns no HSTS; the header\n    is present on the routed API path /v3.0/reporting/publisher.\n  other_headers:\n    x-content-type-options: nosniff\n    x-frame-options: SAMEORIGIN\n    x-xss-protection: 1; mode=block\n    x-dns-prefetch-control: 'off'\n    x-download-options: noopen\n- host: publisher.inmobi.com\n\
  \  role: Ad Management API + publisher dashboard\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: api.cdr.inmobi.com\n  role: DSP Cost API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.w.inmobi.com\n  role: Server-to-Server Ad Request API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: advertising.inmobi.com\n  role: advertiser marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: inmobi.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA record — any public CA may issue for inmobi.com.\n  spf: true\n  spf_policy: '-all (hard fail)'\n  spf_record: 'v=spf1 ip4:50.213.20.161 ip4:209.214.228.18 ip4:101.254.125.194 ip4:123.127.0.146\
  \ include:_s00230767.autospf.email include:outbound.mailhop.org include:2714195.spf01.hubspotemail.net -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 100\n  dmarc_subdomain_policy: quarantine\n  dmarc_rua: dmarc-report@inmobi.com\n  dmarc_ruf: dmarc-report@inmobi.com\nsecurity_txt:\n  published: false\n  probed: 6 hosts, 2026-08-12\n  see: well-known/inmobi-well-known.yml\nvulnerability_disclosure:\n  published: false\n  probes:\n  - {url: 'https://www.inmobi.com/.well-known/security.txt', status: 404}\n  - {url: 'https://www.inmobi.com/security/', status: 200, result: 'security page served but publishes no disclosure policy, contact, or PGP key'}\n  - {url: 'https://hackerone.com/inmobi', status: 404}\n  - {url: 'https://bugcrowd.com/inmobi', status: 404}\n  checked: '2026-08-12'\n  note: >-\n    probe-security-programs.py reported vdp=none on 2026-08-12 and wrote no\n    vulnerability-disclosure artifact, which is the correct outcome. No\n    VulnerabilityDisclosure or\
  \ SecurityTxt pointer is emitted in apis.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inmobi/refs/heads/main/security/inmobi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Mobile
- Monetization
- Programmatic
- OpenRTB
- SDK
- Consent Management
- DSP
- Reporting
---
