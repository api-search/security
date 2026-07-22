---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:CAIssues@sec.gov"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cetera.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: www.cetera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rcs Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RCS Capital, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RCS Capital
provider_slug: rcs-capital
slug: rcs-capital-domain-security
source_filename: rcs-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: www.cetera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cetera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rcs-capital/refs/heads/main/security/rcs-capital-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Broker-Dealer
- Cetera Financial Group
- Defunct
- Financial Services
- Independent Advisor
- Investment Banking
- Wealth Management
---
