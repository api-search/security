---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genalyte.com
  spf: true
hosts:
- cert_expires: Oct  5 21:16:59 2026 GMT
  host: www.genalyte.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genalyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genalyte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Genalyte
provider_slug: genalyte
slug: genalyte-domain-security
source_filename: genalyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genalyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:16:59 2026 GMT\n  hsts: null\ndomains:\n- domain: genalyte.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nx-observations:\n  fetched: '2026-08-04'\n  method: probed\n  note: >-\n    Recorded from live DNS lookups against both the local resolver and 8.8.8.8 on 2026-08-04.\n    Absence of a record is valid observed data, not an inference.\n  unresolved_cnames:\n  - host: api.genalyte.com\n    cname: api.prod.genalyte.com\n    a_records: none\n    http: unreachable\n    note: CNAME target has no A/AAAA record; the API hostname does not resolve to a live host.\n  - host: cloudlab.genalyte.com\n    cname: cloudlab.prod.genalyte.com\n    a_records: none\n    http: unreachable\n    note: CNAME target has no A/AAAA record.\n  - host: lab.genalyte.com\n    cname: d2475hl7gtlu89.cloudfront.net\n\
  \    a_records: none\n    http: unreachable\n    note: >-\n      CNAME points at an Amazon CloudFront distribution that returns no address records,\n      which is consistent with a deleted or disabled distribution.\n  email_posture:\n    spf: present\n    spf_qualifier: '~all (softfail) on the primary record; a second TXT record ends -all'\n    spf_note: >-\n      Two SPF-shaped TXT records are published on genalyte.com, which is a configuration\n      defect under RFC 7208 section 3.2 (a domain must publish exactly one SPF record).\n    dmarc: absent\n    dmarc_note: No _dmarc.genalyte.com TXT record was returned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genalyte/refs/heads/main/security/genalyte-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Medical Devices
- Laboratory
- Point of Care Testing
- Life Sciences
- Biotechnology
- In Vitro Diagnostics
---
