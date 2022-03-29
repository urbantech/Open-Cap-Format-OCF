:house: [Documentation Home](/README.md)

---

### Object - Convertible Conversion Transaction

`https://opencaptablecoalition.com/schema/objects/transactions/conversion/ConvertibleConversion.schema.json`

**Description:** _Object describing a conversion of a convertible security_

**Data Type:** `OCF Object - TX_CONVERTIBLE_CONVERSION`

**Composed From:**

- [schema/primitives/BaseObject](/docs/schema/primitives/BaseObject.md)
- [schema/primitives/transactions/BaseTransaction](/docs/schema/primitives/transactions/BaseTransaction.md)
- [schema/primitives/transactions/conversion/BaseConversion](/docs/schema/primitives/transactions/conversion/BaseConversion.md)

**Properties:**

| Property               | Type                                                                                                                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Required   |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| id                     | `STRING`                                                                                                               | Identifier for the object                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `REQUIRED` |
| comments               | [`STRING`]                                                                                                             | Unstructured text comments related to and stored for the object                                                                                                                                                                                                                                                                                                                                                                                                                                             | -          |
| object_type            | **Constant:** `TX_CONVERTIBLE_CONVERSION`</br>_Defined in [schema/enums/ObjectType](/docs/schema/enums/ObjectType.md)_ | Object type field                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | `REQUIRED` |
| security_id            | `STRING`                                                                                                               | Identifier for the security (stock, plan security, warrant, or convertible) by which it can be referenced by other transaction objects. Note that while this identifier is created with an issuance object, it should be different than the issuance object's `id` field which identifies the issuance transaction object itself. All future transactions on the security (e.g. acceptance, transfer, cancel, etc.) must reference this `security_id` to qualify which security the transaction applies to. | `REQUIRED` |
| date                   | [schema/types/Date](/docs/schema/types/Date.md)                                                                        | Date on which the transaction occurred                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | `REQUIRED` |
| resulting_security_ids | [`STRING`]                                                                                                             | Identifier for the security (or securities) that resulted from the conversion                                                                                                                                                                                                                                                                                                                                                                                                                               | `REQUIRED` |
| reason_text            | `STRING`                                                                                                               | Reason for the conversion                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `REQUIRED` |

**Source Code:** [schema/objects/transactions/conversion/ConvertibleConversion](/schema/objects/transactions/conversion/ConvertibleConversion.schema.json)

**Examples:**

```json
[
  {
    "object_type": "TX_CONVERTIBLE_CONVERSION",
    "id": "test-convertible-conversion-minimal",
    "security_id": "b61c70c8-19a6-49c0-98f4-65f6c76b3841",
    "date": "2006-11-09",
    "reason_text": "for testing",
    "resulting_security_ids": [
      "c349dcc8-cbf9-4ed9-88cd-9de4d0c8517c",
      "..."
    ]
  },
  {
    "object_type": "TX_CONVERTIBLE_CONVERSION",
    "id": "test-convertible-conversion-all-fields",
    "security_id": "b61c70c8-19a6-49c0-98f4-65f6c76b3841",
    "date": "2006-11-09",
    "reason_text": "for testing",
    "resulting_security_ids": [
      "c349dcc8-cbf9-4ed9-88cd-9de4d0c8517c",
      "..."
    ],
    "comments": [
      "comment-one",
      "comment-two",
      "..."
    ]
  }
]
```