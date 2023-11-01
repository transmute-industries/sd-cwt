
## Issued SD-CWT

~~~~ cbor-diag
18(                               / COSE Sign 1 /
  [
    h'A1013822',                  / Protected Header    /
    {                             / Unprotected Header  /
      333: [                      / Disclosures (2)     /
        h'82502BD5...5254494F4E', / Disclosure 1 🔴     /
        h'825091B1...5254494F4E'  / Disclosure 2 🔵     /
      ]
    }, 
    h'AB6566696...61FF6765',      / Payload             /
    h'DCBCDD0C1...11DB6D16'       / Signature           /
  ]
)
~~~~

## Decoded Protected Header

~~~~ cbor-diag
{         / Protected Header /
  1: -35  / alg : ES384      /
}
~~~~

## Decoded Payload
~~~~ cbor-diag
{
  "files": [
    / 🔴 Disclosable Value 1 /
    { 222: h'58F422BA59767BB8DE6BC004D12AF5E888A4D2BCBA95564FF9EFA6D75858A68C' }, 
    {
      "fileName": "./README.md", 
      "SPDXID": "SPDXRef-File--README.md-534A3C13F8D9F8CEBEEC1E452E3D5E53B2B6023A", 
      "checksums": [
        {
          "algorithm": "SHA256", 
          "checksumValue": "2a9467ae0bc2fb767ae582ef954c8811c5140f6eb1b88f6f64f115916764ebf4"
        }, 
        {
          "algorithm": "SHA1", 
          "checksumValue": "534a3c13f8d9f8cebeec1e452e3d5e53b2b6023a"
        }
        ], 
        "licenseConcluded": "NOASSERTION", 
        "licenseInfoInFiles": ["NOASSERTION"], 
        "copyrightText": "NOASSERTION"
      }, 
      {
        "fileName": "./.gitignore", 
        "SPDXID": "SPDXRef-File--.gitignore-1B599299EAB9334A33051A92404B543A3BB41350", 
        "checksums": [
          {
            "algorithm": "SHA256", 
            "checksumValue": "8f5986c32ad03f644673ec102d84cad1f95b3f40fac0da2855c0a2f90eae91e1"
          }, 
          {
            "algorithm": "SHA1", 
            "checksumValue": "1b599299eab9334a33051a92404b543a3bb41350"
            }
        ], 
        "licenseConcluded": "NOASSERTION", 
        "licenseInfoInFiles": ["NOASSERTION"], 
        "copyrightText": "NOASSERTION"
      }, 
      {
        "fileName": "./artifact.js", 
        "SPDXID": "SPDXRef-File--artifact.js-86E48231F3A466D588BEDF5162E4D6FF7B8C0251", 
        "checksums": [
          {
            "algorithm": "SHA256", 
            "checksumValue": "4a3286fb4866f9e48920b6c66090427d0de2db1e79ac2e37a21d29c9518e7c46"
          }, 
          {
            "algorithm": "SHA1", 
            "checksumValue": "86e48231f3a466d588bedf5162e4d6ff7b8c0251"
            }
        ], 
        "licenseConcluded": "NOASSERTION", 
        "licenseInfoInFiles": ["NOASSERTION"], 
        "copyrightText": "NOASSERTION"
      }, 
      {
        "fileName": "./package.json", 
        "SPDXID": "SPDXRef-File--package.json-8EE24E0660E30C48D31317534400CCFBC149CB75", 
        "checksums": [
          {
            "algorithm": "SHA256", 
            "checksumValue": "fb97d8cc1e12227be8e5b7c64d47b71fab407a3820871da25825e734b6ae97d7"
          }, 
          {
            "algorithm": "SHA1", 
            "checksumValue": "8ee24e0660e30c48d31317534400ccfbc149cb75"
          }
        ], 
        "licenseConcluded": "NOASSERTION", 
        "licenseInfoInFiles": ["NOASSERTION"], 
        "copyrightText": "NOASSERTION"
      }, 
      / 🔵 Disclosable Value 2 /
      { 222: h'7DE993F9918D0A14B0FC2A15D041DFEC0C37CEE46926DBDFB0453C3A1C833B44' }
  ], 
  "packages": [
    {
      "name": "scitt-nodejs-example",
      "SPDXID": "SPDXRef-RootPackage",
      "downloadLocation": "NOASSERTION",
      "packageVerificationCode": {
        "packageVerificationCodeValue": "8277f9ac2e97a0feb01186977e63ac432556bfe5"
      },
      "filesAnalyzed": true,
      "licenseConcluded": "NOASSERTION",
      "licenseInfoFromFiles": [
        "NOASSERTION"
      ],
      "licenseDeclared": "NOASSERTION",
      "copyrightText": "NOASSERTION",
      "versionInfo": "0.0.0",
      "externalRefs": [
        {
          "referenceCategory": "PACKAGE-MANAGER",
          "referenceType": "purl",
          "referenceLocator": "pkg:swid/scitt-community/spdx.org/scitt-nodejs-example@0.0.0?tag_id=44c701aa-7829-4bc5-9fff-099c001ae300"
        }
      ],
      "supplier": "Organization: scitt-community",
      "hasFiles": [
        "SPDXRef-File--script.sh-A5BE2A0E0FC9F8C2DA4F420B3046CD292AFB11C5",
        "SPDXRef-File--artifact.js-86E48231F3A466D588BEDF5162E4D6FF7B8C0251",
        "SPDXRef-File--package.json-8EE24E0660E30C48D31317534400CCFBC149CB75",
        "SPDXRef-File--clean.sh-49B0B794639658A24ED0F30BCCC4124A886FA908",
        "SPDXRef-File--.gitignore-1B599299EAB9334A33051A92404B543A3BB41350",
        "SPDXRef-File--README.md-534A3C13F8D9F8CEBEEC1E452E3D5E53B2B6023A"
      ]
    }
  ],
  "externalDocumentRefs": [],
  "relationships": [
    {
      "relationshipType": "DESCRIBES",
      "relatedSpdxElement": "SPDXRef-RootPackage",
      "spdxElementId": "SPDXRef-DOCUMENT"
    }
  ],
  "spdxVersion": "SPDX-2.2",
  "dataLicense": "CC0-1.0",
  "SPDXID": "SPDXRef-DOCUMENT",
  "name": "scitt-nodejs-example 0.0.0",
  "documentNamespace": "https://spdx.org/spdxdocs/sbom-tool-1.7.1-b4b2627e-c28a-4c65-8f00-8a79cfedc225/scitt-nodejs-example/0.0.0/PWJovljzU0qFaGdHRWqKDg",
  "creationInfo": {
    "created": "2023-11-01T17:26:46Z",
    "creators": [
      "Organization: scitt-community",
      "Tool: Microsoft.SBOMTool-1.7.1"
    ]
  },
  "documentDescribes": [ "SPDXRef-RootPackage" ]
}
~~~~


## Disclosure 1

~~~~ cbor-diag
[
  h'2BD5D126E016912A103D7B0B1B233AC6', / Salt / 
  { / 🔴 Disclosed Value 1 / 
    "fileName": "./script.sh", 
    "SPDXID": "SPDXRef-File--script.sh-A5BE2A0E0FC9F8C2DA4F420B3046CD292AFB11C5", 
    "checksums": [
      {
        "algorithm": "SHA256", 
        "checksumValue": "e12fc416bf4aebf08117725577e05900aabf7ba7bda1c05e78cb519620c9a0b6"
      }, 
      {
        "algorithm": "SHA1", 
        "checksumValue": "a5be2a0e0fc9f8c2da4f420b3046cd292afb11c5"
      }
    ], 
    "licenseConcluded": "NOASSERTION", 
    "licenseInfoInFiles": ["NOASSERTION"], 
    "copyrightText": "NOASSERTION"
  }
]
~~~~

## Disclosure 2

~~~~ cbor-diag
[
  h'91B103A152F115724C576344D268371B',   / Salt / 
  { / 🔵 Disclosed Value 2 /
    "fileName": "./clean.sh", 
    "SPDXID": "SPDXRef-File--clean.sh-49B0B794639658A24ED0F30BCCC4124A886FA908", 
    "checksums": [
      {
        "algorithm": "SHA256", 
        "checksumValue": "a42c14e6502ccbc2a8abd051bd38fe1037f40e6084afb667a87bb59572c89657"
      }, 
      {
        "algorithm": "SHA1", 
        "checksumValue": "49b0b794639658a24ed0f30bccc4124a886fa908"
        }
    ], 
    "licenseConcluded": "NOASSERTION", 
    "licenseInfoInFiles": ["NOASSERTION"], 
    "copyrightText": "NOASSERTION"
  }
]
~~~~