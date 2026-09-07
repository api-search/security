---
description: ''
domains:
- a_records:
  - 75.2.103.146
  - 99.83.188.150
  caa:
    present: true
    records:
    - 0 issue "www.digicert.com"
    - 0 issue "letsencrypt.org"
    - 0 iodef "mailto:secops@dfamilk.com"
  created: '1997-04-04'
  dmarc:
    aggregate_reporting: true
    forensic_reporting: true
    policy: reject
    present: true
    record: v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com
  dnssec:
    ds_records: []
    signed: false
  domain: deanfoods.com
  domain_status:
  - clientTransferProhibited
  hsts:
    header: null
    note: Cannot be served — there is no working HTTPS response to carry the header.
    present: false
  http:
    behavior: blanket 301 to https://www.dfamilk.com/ on every path tested
    head_method: 405 Method Not Allowed (WAF in front of the ELB refuses HEAD)
    listener: true
    server: awselb/2.0
  mx:
    present: true
    records:
    - 10 mxa-004c8e03.gslb.pphosted.com
    - 10 mxb-004c8e03.gslb.pphosted.com
  nameservers:
  - ns11.gcd-dns.com
  - ns12.gcd-dns.com
  registrant_organization: Dairy Farmers of America, Inc.
  registrar: GoDaddy Corporate Domains, LLC
  registry_expiry: '2027-04-05'
  resolves: true
  spf:
    all_qualifier: softfail
    note: Proofpoint macro-expanded SPF include — the same tenant DFA uses.
    present: true
    record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all
  tls:
    certificate: null
    error: tlsv1 alert internal error (LibreSSL ST_CONNECT)
    handshake: failed
    https_listener: false
    note: Port 443 accepts the connection but aborts the TLS handshake, so no certificate can be retrieved and no https:// request to this host can complete. Every https probe in this repo against deanfoods.com is therefore status 0 — no connection, not a 404.
  updated: '2026-03-08'
hosts: []
hosts_probed: 0
kind: domain-security
layout: security
method: probed
name: Dean Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dean Foods, probed live across 0 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Dean Foods
provider_slug: dean-foods
slug: dean-foods-domain-security
source_filename: dean-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: DNS + TLS probe of deanfoods.com, 2026-09-05\n\n# Dean Foods — domain security posture of deanfoods.com.\n#\n# ATTRIBUTION, READ THIS FIRST. Dean Foods ceased to exist as an operating company\n# after its 2019 Chapter 11 filing and the 2020 sale of its assets. The registrant of\n# record on deanfoods.com is now DAIRY FARMERS OF AMERICA, INC., and the CAA iodef\n# contact is secops@dfamilk.com — so the posture measured below is the ACQUIRER's\n# stewardship of an inherited brand domain, not a security program Dean Foods runs.\n# It is recorded because deanfoods.com is the domain this record names, and because\n# the shape of it (mail hardened, web abandoned) is itself the evidence that the\n# company is gone: a domain kept alive for mail and brand defence, with no HTTPS\n# listener at all.\n\nname: Dean Foods\nslug: dean-foods\nchecked: '2026-09-05'\nhosts_probed:\n- deanfoods.com\n\ndomains:\n- domain: deanfoods.com\n  registrar:\
  \ GoDaddy Corporate Domains, LLC\n  registrant_organization: Dairy Farmers of America, Inc.\n  created: '1997-04-04'\n  updated: '2026-03-08'\n  registry_expiry: '2027-04-05'\n  domain_status:\n  - clientTransferProhibited\n  resolves: true\n  a_records:\n  - 75.2.103.146\n  - 99.83.188.150\n  nameservers:\n  - ns11.gcd-dns.com\n  - ns12.gcd-dns.com\n\n  tls:\n    https_listener: false\n    handshake: failed\n    error: 'tlsv1 alert internal error (LibreSSL ST_CONNECT)'\n    certificate: null\n    note: >-\n      Port 443 accepts the connection but aborts the TLS handshake, so no certificate\n      can be retrieved and no https:// request to this host can complete. Every\n      https probe in this repo against deanfoods.com is therefore status 0 —\n      no connection, not a 404.\n  hsts:\n    present: false\n    header: null\n    note: Cannot be served — there is no working HTTPS response to carry the header.\n  http:\n    listener: true\n    behavior: blanket 301 to https://www.dfamilk.com/\
  \ on every path tested\n    server: awselb/2.0\n    head_method: 405 Method Not Allowed (WAF in front of the ELB refuses HEAD)\n\n  dnssec:\n    signed: false\n    ds_records: []\n  caa:\n    present: true\n    records:\n    - '0 issue \"www.digicert.com\"'\n    - '0 issue \"letsencrypt.org\"'\n    - '0 iodef \"mailto:secops@dfamilk.com\"'\n  spf:\n    present: true\n    record: 'v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all'\n    all_qualifier: softfail\n    note: Proofpoint macro-expanded SPF include — the same tenant DFA uses.\n  dmarc:\n    present: true\n    record: 'v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com'\n    policy: reject\n    aggregate_reporting: true\n    forensic_reporting: true\n  mx:\n    present: true\n    records:\n    - 10 mxa-004c8e03.gslb.pphosted.com\n    - 10 mxb-004c8e03.gslb.pphosted.com\n\nsummary:\n  email_authentication: strong\n  web_transport: absent\n  finding:\
  \ >-\n    An asymmetric posture that is diagnostic of a wound-down brand: SPF, DMARC at\n    p=reject with both aggregate and forensic reporting, CAA with a named security\n    contact, and live Proofpoint MX — all of the controls that stop someone spoofing\n    mail from a well-known dead brand — combined with no HTTPS service whatsoever and\n    a plain-HTTP blanket redirect to the acquirer. The domain is being defended, not\n    operated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dean-foods/refs/heads/main/security/dean-foods-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Acquired
- Beverages
- Dairy
- Defunct
- Food and Beverage
- Milk
- Fortune 500
---
