### CIA Triad

![Confidentiality, Integrity, and Availability are the three principles driving information security.](https://assets.wgu.edu/5d0894ad92b36c295e1f0ecc5ea41ff7)

Diagram: The CIA Triad

Consistency is critical in security management; therefore, some organizations create specific classifications for their data that define different sensitivity levels, each with specific policies that explain how the information should be handled. These classification levels are then applied to every file, email, database, and even printed papers. When evaluating the sensitivity of a piece of information, all three of the CIA principles should be taken into consideration; however, depending on the type of information, you may focus more on one principle than another.

### Confidentiality

The confidentiality principle helps limit access to information, which, by definition, can contradict some of the recommendations found in the availability principle. The goal of confidentiality is to prevent an unauthorized user from accessing, copying, or transmitting the information.

Confidentiality is often equated to privacy because the two terms share many of the same characteristics, such as ensuring that only the intended recipient of the information can access it, following a need-to-know policy, and reducing exposure by destroying all copies of the information that are no longer needed.

There are many ways to breach or compromise the confidentiality of data if the proper precautions are not taken in advance and then routinely checked for accuracy and consistency.

-   Unencrypted information is easy to steal and change.
-   Deleted files are rarely purged from a disk immediately and often can be recovered with ease.
-   The physical theft of a device gives an attacker an unlimited time window to break the encryption of your data.
-   Social engineering is a method used by attackers to gain an unsuspecting victim’s trust to provide information, such as passwords or server names, or even just to gain physical building access.
-   Accidents and malfunctions also play into the equation. For example, confidentiality of information can easily be breached by storing files in the wrong location, emailing data to the wrong person, or printing confidential information to a public printer.

Some methods that may help prevent compromises include:

-   Where possible, encrypt the information at-rest (where it is stored) and in-transit (while it is moving across the network).
-   Be sure to encrypt and physically secure your laptops, servers, portable hard drives, and even backup tapes/disks.
-   Consider using a tool to securely delete files or overwrite them after deletion.
-   Train your employees about social engineering attacks.
-   Create and enforce a policy that ensures all users must use complex passwords (a combination of uppercase and lowercase letters, numbers, and symbols with a minimum length) and use multifactor authentication (MFA), such as biometrics or a digital key fob.
-   Following the principle of least privilege (which means you only assign users the minimum permissions needed to perform their jobs), institute restrictive access controls on all data and provide access to information on a need-to-know basis only.

### Integrity

The integrity principle helps identify the trustworthiness of the information. It is possible to identify where the information came from and if the data has changed since it was originally sent. Integrity is a function that is often incorporated into encryption and, therefore, works well with the confidentiality principle.

Some of the compromises of data integrity include:

-   Man-in-the-middle attacks, where an attacker changes the contents of the message after it was sent, but before it was received
-   The intentional or unintentional deletion or modification of data
-   Malfunctions in equipment that cause data corruption
-   Natural phenomena such as electromagnetic pulse (EMP) attacks, which can destroy or severely corrupt data

Some methods that can be employed to help prevent the compromise of data integrity include:

-   Require all data transmissions to use encryption or digital signatures to confirm the identity of the sender and to identify if the message has been changed.
-   In cases where digital signatures will not work, use one-way hash calculations, such as SHA-3 (Secure Hash Algorithm 3), to create a value that can be used to verify the data has not changed.
-   Use version control within your data storage to help you quickly revert accidental changes or deletions.

### Availability

The goal of the availability principle is to ensure that the data is always accessible by its authorized users. This includes aspects such as adding high availability to your server solutions and minimizing downtime by carefully managing your application updates and patches.

Some of the common actions that can compromise the availability of data include:

-   denial-of-service (DoS) and distributed denial-of-service (DDoS) attacks, which prevent legitimate users from accessing the resource by sending an overwhelming amount of data to the target server;
-   unplanned downtime due to server crashes or failed upgrades; and
-   accidental changes to access control lists, which removes access for authorized users.

Some methods that can be employed to help prevent availability issues include:

-   creating and maintaining a full disaster recovery plan that includes a full site failover as well as the method to restore data for individual servers;
-   implementing server high availability where possible, employing clustering technology where appropriate; and
-   setting up regular backups of your data and considering storing a backup copy at another physical location to protect against site-level disasters.