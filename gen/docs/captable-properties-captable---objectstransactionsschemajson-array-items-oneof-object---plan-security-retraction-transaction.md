# Object - Plan Security Retraction Transaction Schema

```txt
Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/transactions/items/oneOf/17
```

Object describing a retraction of a plan security

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [CapTable.schema.json*](../../schema/CapTable.schema.json "open original schema") |

## 17 Type

`object` ([Object - Plan Security Retraction Transaction](captable-properties-captable---objectstransactionsschemajson-array-items-oneof-object---plan-security-retraction-transaction.md))

all of

*   all of

    *   all of

        *   [Object - BaseObject](issuer-allof-object---baseobject.md "check type definition")

# 17 Properties

| Property                    | Type          | Required | Nullable       | Defined by                                                                                                                                                                                     |
| :-------------------------- | :------------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [object_type](#object_type) | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-object_type.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/object_type") |
| [id](#id)                   | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-id.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/id")                   |
| [comments](#comments)       | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-comments.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/comments")       |
| [security_id](#security_id) | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-security_id.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/security_id") |
| [date](#date)               | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-date.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/date")               |
| [reason_text](#reason_text) | Not specified | Optional | cannot be null | [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-reason_text.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/reason_text") |

## object_type



`object_type`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-object_type.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/object_type")

### object_type Type

unknown

### object_type Constraints

**constant**: the value of this property must be equal to:

```json
"TX_PLAN_SECURITY_RETRACTION"
```

## id



`id`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-id.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/id")

### id Type

unknown

## comments



`comments`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-comments.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/comments")

### comments Type

unknown

## security_id



`security_id`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-security_id.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/security_id")

### security_id Type

unknown

## date



`date`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-date.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/date")

### date Type

unknown

## reason_text



`reason_text`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Plan Security Retraction Transaction](plansecurityretraction-properties-reason_text.md "Objects.Transactions.Retraction.PlanSecurityRetraction.schema.json#/properties/reason_text")

### reason_text Type

unknown