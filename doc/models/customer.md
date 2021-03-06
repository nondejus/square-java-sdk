## Customer

Represents a Square customer profile, which can have one or more
cards on file associated with it.

### Structure

`Customer`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `String` | Optional | A unique Square-assigned ID for the customer profile. |
| `CreatedAt` | `String` | Optional | The timestamp when the customer profile was created, in RFC 3339 format. |
| `UpdatedAt` | `String` | Optional | The timestamp when the customer profile was last updated, in RFC 3339 format. |
| `Cards` | [`List<Card>`](/doc/models/card.md) | Optional | Payment details of cards stored on file for the customer profile. |
| `GivenName` | `String` | Optional | The given (i.e., first) name associated with the customer profile. |
| `FamilyName` | `String` | Optional | The family (i.e., last) name associated with the customer profile. |
| `Nickname` | `String` | Optional | A nickname for the customer profile. |
| `CompanyName` | `String` | Optional | A business name associated with the customer profile. |
| `EmailAddress` | `String` | Optional | The email address associated with the customer profile. |
| `Address` | [`Address`](/doc/models/address.md) | Optional | Represents a physical address. |
| `PhoneNumber` | `String` | Optional | The 11-digit phone number associated with the customer profile. |
| `Birthday` | `String` | Optional | The birthday associated with the customer profile, in RFC-3339 format.<br>Year is optional, timezone and times are not allowed.<br>For example: `0000-09-01T00:00:00-00:00` indicates a birthday on September 1st.<br>`1998-09-01T00:00:00-00:00` indications a birthday on September 1st __1998__. |
| `ReferenceId` | `String` | Optional | An optional, second ID used to associate the customer profile with an<br>entity in another system. |
| `Note` | `String` | Optional | A custom note associated with the customer profile. |
| `Preferences` | [`CustomerPreferences`](/doc/models/customer-preferences.md) | Optional | Represents communication preferences for the customer profile. |
| `Groups` | [`List<CustomerGroupInfo>`](/doc/models/customer-group-info.md) | Optional | The customer groups and segments the customer belongs to. This deprecated field has been replaced with  the dedicated `group_ids` for customer groups and the dedicated `segment_ids` field for customer segments. You can retrieve information about a given customer group and segment respectively using the Customer Groups API and Customer Segments API. |
| `CreationSource` | [`String`](/doc/models/customer-creation-source.md) | Optional | Indicates the method used to create the customer profile. |
| `GroupIds` | `List<String>` | Optional | The IDs of customer groups the customer belongs to. |
| `SegmentIds` | `List<String>` | Optional | The IDs of segments the customer belongs to. |

### Example (as JSON)

```json
{
  "id": null,
  "created_at": null,
  "updated_at": null,
  "cards": null,
  "given_name": null,
  "family_name": null,
  "nickname": null,
  "company_name": null,
  "email_address": null,
  "address": null,
  "phone_number": null,
  "birthday": null,
  "reference_id": null,
  "note": null,
  "preferences": null,
  "groups": null,
  "creation_source": null,
  "group_ids": null,
  "segment_ids": null
}
```

