---
certifications: []
description: ''
kind: trust-center
layout: security
name: May Mobility Trust Center
name_suffix: Trust Center
overview: May Mobility maintains a public trust center covering its security and compliance posture.
provider_name: May Mobility
provider_slug: may-mobility
slug: may-mobility-trust-center
source_filename: may-mobility-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://may-mobility.trustshare.com/home\nplatform: TrustShare (TrustCloud Corporation)\nlanding_page: https://maymobility.com/cybersecurity/\nprogram:\n  name: Trust and Compliance Program\n  description: 'May Mobility publishes its security and compliance program through a\n    hosted TrustShare instance. The public cybersecurity page states the program is\n    surfaced as \"a real-time feed from the compliance program in Trust Cloud\" and\n    that May Mobility \"continuously monitor, test, improve, and share our security\n    and compliance program\".'\ncertifications: []\ncertifications_note: 'The TrustShare portal at https://may-mobility.trustshare.com/home\n  returns HTTP 200 but is a client-rendered single-page application; no certification\n  names (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP, GDPR, ISO 21434, TISAX) could be\n  read from the server-rendered response, and no certification list is published\
  \ on\n  maymobility.com/cybersecurity/ itself. Certifications are therefore recorded as\n  UNVERIFIED rather than asserted. Individual documents on TrustShare portals are\n  commonly gated behind an NDA request flow. Re-probe with a rendering fetch to\n  confirm.'\nnetwork_trust:\n  note: 'Separately from the TrustShare portal, May Mobility publishes an operational\n    trust surface on its NOC documentation site covering the networks and PKI it\n    operates. This is a real, verbatim-published artifact and is recorded here\n    because it is the only certification-grade security detail May Mobility puts in\n    the open.'\n  operated_networks_url: https://net.maymobility.com/docs/network/trust\n  operated_ipv4:\n  - 66.51.148.0/24\n  operated_ipv6:\n  - 2602:80a:2000::/40\n  - 2607:f790:fff6::/48\n  operated_domains:\n  - domain: maymobility.com\n    use: public\n  - domain: maymobility.net\n    use: backbone and internal network\n  certificates_url: https://net.maymobility.com/docs/network/certs\n\
  \  internal_pki:\n    root_ca: May Mobility Root CA ECC US2 (Ann Arbor, Michigan)\n    intermediates:\n    - May Mobility Intermediate CA ECC US2\n    - May Mobility Intermediate CA ECC SLC (client certificates)\n    key_algorithm: ECDSA P256\n    signing_algorithm: SHA256 ECDSA\n    key_storage_standard: FIPS 140-2 level 3 or higher\n    ocsp: http://ocsp.its.maymobility.com\n    published_pem: true\n    published_pem_note: Root and both intermediate CA certificates are published in\n      full PEM form on the certs page.\n  autonomous_system:\n    asn: 398351\n    org: May Mobility, Inc\n    peeringdb: https://www.peeringdb.com/net/23152\n    irr_as_set: RADB::AS-MAYMOBILITY\n    peering_policy: https://net.maymobility.com/docs/policies/peering\n    looking_glass: https://lg.net.maymobility.com/\n    abuse_contact: abuse@maymobility.com\nevidence:\n- source: https://maymobility.com/cybersecurity/\n  http_status: 200\n  keywords:\n  - trust and compliance program\n  - security and compliance\n\
  \  - trustshare\n  - trust cloud\n- source: https://may-mobility.trustshare.com/home\n  http_status: 200\n  note: JavaScript-rendered SPA shell; no compliance detail in the HTML response.\n- source: https://net.maymobility.com/docs/network/trust\n  http_status: 200\n- source: https://net.maymobility.com/docs/network/certs\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/may-mobility/refs/heads/main/security/may-mobility-trust-center.yml
summary_line: trust center published
tags:
- Company
- Autonomous Vehicles
- Transportation
- Mobility
- Robotaxi
- Fleet Management
- Telemetry
- Public Transit
- Automotive
- Streaming
trust_url: https://may-mobility.trustshare.com/home
---
