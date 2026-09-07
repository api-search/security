---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altrubio.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: abgenomics.com
  note: SPF present but is the parking service's null-route record ("v=spf1 ip6:fdcf:abda:4154::/48 -all"), not a mail configuration the company operates. No DNSKEY, no CAA, no _dmarc record.
  spf: true
hosts:
- cert_expires: Nov 25 10:13:57 2026 GMT
  host: www.altrubio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: null
  host: abgenomics.com
  hsts: false
  https: true
  note: The company's original registrable domain. HTTPS answered 200 on the first probes of this pass (abovedomains.com parking page, 1,005 bytes), then the origin began timing out connections on repeat requests, so TLS version and certificate expiry could not be read. This is the parking service's posture, not the company's — abgenomics.com is delegated to ns1/ns2.abovedomains.com and advertises "This domain may be for sale".
  tls_version: null
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Abgenomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abgenomics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abgenomics
provider_slug: abgenomics
slug: abgenomics-domain-security
source_filename: abgenomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altrubio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 10:13:57 2026 GMT\n  hsts: false\n- host: abgenomics.com\n  https: true\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  note: >-\n    The company's original registrable domain. HTTPS answered 200 on the first probes of this\n    pass (abovedomains.com parking page, 1,005 bytes), then the origin began timing out\n    connections on repeat requests, so TLS version and certificate expiry could not be read.\n    This is the parking service's posture, not the company's — abgenomics.com is delegated to\n    ns1/ns2.abovedomains.com and advertises \"This domain may be for sale\".\ndomains:\n- domain: altrubio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: abgenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n\
  \  dmarc_policy: null\n  note: >-\n    SPF present but is the parking service's null-route record (\"v=spf1 ip6:fdcf:abda:4154::/48\n    -all\"), not a mail configuration the company operates. No DNSKEY, no CAA, no _dmarc record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abgenomics/refs/heads/main/security/abgenomics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Therapeutics
- Clinical Research
- Immunology
- Oncology
---
