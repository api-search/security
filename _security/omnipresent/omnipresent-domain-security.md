---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: omnipresent.com
  ds_records: 0
  mx: true
  mx_provider: Google Workspace (aspmx.l.google.com)
  nameservers:
  - ns-45.awsdns-05.com
  - ns-559.awsdns-05.net
  - ns-1069.awsdns-05.org
  - ns-1626.awsdns-11.co.uk
  note: Mail is still delegated to Google Workspace while the web is gone. No SPF TXT record and no _dmarc TXT record are published, so a live mail domain is running with no published sender authentication or reporting policy — the notable finding here.
  spf: false
  zone_present: true
- caa: null
  dmarc: null
  dnssec: null
  domain: omnipresent.group
  mx: null
  note: SERVFAIL on every query; delegation is broken or the registration has lapsed.
  spf: null
  zone_present: false
hosts:
- dns_a_records: 0
  host: https://omnipresent.com
  https: false
  note: Apex has NS delegation to Route 53 but publishes no A or AAAA record; every HTTPS request fails at name resolution (curl exit 6), so no certificate, TLS version or HSTS header can be observed.
  reachable: false
- dns_a_records: 0
  host: https://www.omnipresent.com
  https: false
  note: NXDOMAIN — the www label was removed from the zone.
  reachable: false
- dns_a_records: 0
  host: https://omnipresent.group
  https: false
  note: The company's original domain. Delegation is broken at the registry — every public resolver returns SERVFAIL — so the zone no longer answers at all.
  reachable: false
kind: domain-security
layout: security
method: probed
name: Omnipresent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omnipresent, probed live across 3 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Omnipresent
provider_slug: omnipresent
slug: omnipresent-domain-security
source_filename: omnipresent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of omnipresent.com and omnipresent.group, 2026-08-26\nnote: >-\n  This file was first written by probe-domain-security.py against www.hiive.com — the\n  secondary-market VENUE listed in apis.yml, not a host Omnipresent controls — and was\n  rewritten by hand so the posture recorded here belongs to the company. Omnipresent was\n  acquired by Deel in October 2025 and its web presence has been decommissioned: neither\n  omnipresent.com nor omnipresent.group serves anything over HTTP, so there is no TLS or\n  HSTS posture left to measure. The Google Workspace MX records on omnipresent.com are\n  still published, which is why the zone still exists at all.\nhosts:\n- host: https://omnipresent.com\n  reachable: false\n  https: false\n  dns_a_records: 0\n  note: >-\n    Apex has NS delegation to Route 53 but publishes no A or AAAA record; every HTTPS\n    request fails at name resolution (curl exit 6), so no\
  \ certificate, TLS version or\n    HSTS header can be observed.\n- host: https://www.omnipresent.com\n  reachable: false\n  https: false\n  dns_a_records: 0\n  note: NXDOMAIN — the www label was removed from the zone.\n- host: https://omnipresent.group\n  reachable: false\n  https: false\n  dns_a_records: 0\n  note: >-\n    The company's original domain. Delegation is broken at the registry — every public\n    resolver returns SERVFAIL — so the zone no longer answers at all.\ndomains:\n- domain: omnipresent.com\n  zone_present: true\n  nameservers:\n  - ns-45.awsdns-05.com\n  - ns-559.awsdns-05.net\n  - ns-1069.awsdns-05.org\n  - ns-1626.awsdns-11.co.uk\n  dnssec: false\n  ds_records: 0\n  caa: []\n  mx: true\n  mx_provider: Google Workspace (aspmx.l.google.com)\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  note: >-\n    Mail is still delegated to Google Workspace while the web is gone. No SPF TXT record\n    and no _dmarc TXT record are published, so a live mail domain is running\
  \ with no\n    published sender authentication or reporting policy — the notable finding here.\n- domain: omnipresent.group\n  zone_present: false\n  dnssec: null\n  caa: null\n  mx: null\n  spf: null\n  dmarc: null\n  note: SERVFAIL on every query; delegation is broken or the registration has lapsed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnipresent/refs/heads/main/security/omnipresent-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Human Resources
- Employment
- Payroll
- Employer of Record
- Global Employment
- Remote Work
- Compliance
- Benefits
- Acquired
- Defunct
---
