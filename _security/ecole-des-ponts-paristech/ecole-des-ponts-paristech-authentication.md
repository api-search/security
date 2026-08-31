---
api_key_in: []
auth_types: []
description: 'How authentication works across the surfaces attributed to École des Ponts ParisTech. There is no API key programme, no developer registration and no OAuth client provisioning anywhere on an ENPC host. What ENPC does operate is campus identity: a SAML 2.0 Identity Provider registered in the French national research and education federation, and a CAS server. Both authenticate people into institutional applications; neither issues credentials to third-party developers.'
kind: authentication
layout: security
method: probed
name: Ecole Des Ponts Paristech Authentication
name_suffix: Authentication
oauth_flows: []
overview: École des Ponts ParisTech declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: École des Ponts ParisTech
provider_slug: ecole-des-ponts-paristech
scheme_count: 0
schemes: []
slug: ecole-des-ponts-paristech-authentication
source_filename: ecole-des-ponts-paristech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\naid: ecole-des-ponts-paristech\nname: École des Ponts ParisTech — Authentication\ndescription: >-\n  How authentication works across the surfaces attributed to École des Ponts\n  ParisTech. There is no API key programme, no developer registration and no OAuth\n  client provisioning anywhere on an ENPC host. What ENPC does operate is campus\n  identity: a SAML 2.0 Identity Provider registered in the French national research\n  and education federation, and a CAS server. Both authenticate people into\n  institutional applications; neither issues credentials to third-party developers.\ngenerated: '2026-08-30'\nmethod: probed\nsource: live HTTP probes against idp.enpc.fr, cas.enpc.fr and the RENATER federation metadata, 2026-08-30\nmechanisms:\n  - type: saml2\n    name: ENPC SAML 2.0 Identity Provider\n    x-operator: institution\n    entity_id: https://idp.enpc.fr/saml/metadata\n    metadata_url: https://idp.enpc.fr/saml/metadata\n    software: LemonLDAP::NG\n    federation:\
  \ RENATER Fédération Éducation-Recherche (member of eduGAIN)\n    endpoints:\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n        purpose: SingleSignOn\n        location: https://idp.enpc.fr/saml/singleSignOn\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n        purpose: SingleSignOn\n        location: https://idp.enpc.fr/saml/singleSignOn\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Artifact\n        purpose: SingleSignOn\n        location: https://idp.enpc.fr/saml/singleSignOnArtifact\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n        purpose: SingleLogout\n        location: https://idp.enpc.fr/saml/singleLogout\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n        purpose: ArtifactResolution\n        location: https://idp.enpc.fr/saml/artifact\n    audience: staff, students and federated service providers — not third-party developers\n    evidence:\n      - url: https://idp.enpc.fr/saml/metadata\n\
  \        status: 200\n      - url: https://metadata.federation.renater.fr/renater/main/main-idps-renater-metadata.xml\n        status: 200\n        note: contains entityID=\"https://idp.enpc.fr/saml/metadata\"\n  - type: cas\n    name: ENPC CAS server\n    x-operator: institution\n    login_url: https://cas.enpc.fr/cas/login\n    detail: >-\n      A CAS login server branded \"École des ponts et chaussées\" fronts internal\n      applications. CAS ticket validation is machine-readable by protocol, but no\n      public service registration exists, so it is not a developer-accessible surface.\n    evidence:\n      - url: https://cas.enpc.fr/cas/login\n        status: 200\n  - type: microsoft-entra\n    name: Microsoft 365 / SharePoint intranet sign-in\n    x-operator: vendor\n    detail: >-\n      intranet.enpc.fr redirects to login.microsoftonline.com for tenant\n      cbc292d3-d274-4204-9169-16847b678004 and resolves to enpcfr.sharepoint.com.\n      Vendor-operated staff intranet, recorded\
  \ for completeness only. Not a surface.\n    evidence:\n      - url: https://intranet.enpc.fr/\n        status: 200\n        note: redirects to login.microsoftonline.com, SharePoint Online tenant enpcfr\nnot_present:\n  - api_keys: no API key issuance, developer account, or self-service credential flow on any ENPC host\n  - oauth2: >-\n      No OAuth 2.0 authorization server. /.well-known/openid-configuration and\n      /oauth2/.well-known/openid-configuration on idp.enpc.fr both return the\n      LemonLDAP::NG portal HTML — soft-200s, not discovery documents.\n  - developer_portal: no api.enpc.fr, api.ecoledesponts.fr or developer portal resolves\npublic_surfaces_requiring_no_auth:\n  - https://idp.enpc.fr/saml/metadata\n  - https://heritage.ecoledesponts.fr/iiif/ark:/12148/btv1b104842475/manifest.json\n  - https://api.archives-ouvertes.fr/search/ENPC/\n  - https://entrepot.recherche.data.gouv.fr/api/dataverses/ecoledesponts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecole-des-ponts-paristech/refs/heads/main/authentication/ecole-des-ponts-paristech-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Technical University
- Grande École
- Engineering
- France
- Research
- Open Access
- Research Data
- Identity Federation
- Digital Library
- OAI-PMH
- IIIF
- SAML
---
