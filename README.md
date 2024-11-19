# Database Attributes Documentation

This document provides an overview of the **current attributes** in our database and the **additional attributes** that are desired for future implementation. 

---

## Current Attributes

The following attributes are currently implemented in the database:

| **Attribute Name** | **Displayed Name (Title)** | **Data Type** | **Description**                               | **Example**            |
|---------------------|----------------------------|---------------|-----------------------------------------------|------------------------|
| `id`               | ID                         | Integer       | Unique identifier for each record.            | `101`                 |
| `name`             | Name                       | String        | Name of the entity (user, product, etc.).     | `John Doe`            |
| `email`            | Email                      | String        | Email address for communication.              | `example@email.com`   |
| `created_at`       | Created At                 | Timestamp     | Record creation timestamp.                    | `2024-11-01 12:00:00` |
| `updated_at`       | Updated At                 | Timestamp     | Last updated timestamp.                       | `2024-11-15 08:30:00` |

---

## Desired Attributes

To improve the functionality of the database, the following attributes are proposed:

| **Attribute Name**  | **Displayed Name (Title)** | **Data Type** | **Description**                               | **Example**            |
|----------------------|----------------------------|---------------|-----------------------------------------------|------------------------|
| `phone_number`      | Phone Number               | String        | Contact phone number for the entity.          | `+1-800-123-4567`     |
| `address`           | Address                    | String        | Full mailing address.                         | `123 Main St, City`   |
| `status`            | Status                     | Enum          | Current status of the record (e.g., active, inactive). | `active`             |
| `profile_picture`   | Profile Picture            | String (URL)  | Link to the profile picture.                  | `https://.../image.jpg`|
| `role`              | Role                       | String        | Role assigned to the entity (e.g., admin, user). | `admin`              |
| `last_login`        | Last Login                 | Timestamp     | Timestamp of the last login.                  | `2024-11-18 22:15:00` |
| `preferences`       | Preferences                | JSON          | User preferences for customizable settings.   | `{"theme":"dark"}`    |

---

## Notes and Considerations

- **Backward Compatibility**: Adding these attributes will not disrupt existing records; default values will be provided where necessary.
- **Security Measures**: Sensitive information such as `phone_number` and `address` will be encrypted or masked in public-facing applications.
- **Testing**: Ensure robust testing is carried out for all new attributes to prevent data integrity issues.

---

## How to Contribute

If you have suggestions or additional desired attributes, please follow these steps:

1. Fork the repository.
2. Make your changes to this document or related files.
3. Submit a pull request explaining the proposed updates.
