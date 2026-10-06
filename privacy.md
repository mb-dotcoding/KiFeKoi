# Privacy Policy

**Last updated: 6 October 2026**

[Version française](confidentialite.html) · [Terms of Use](terms.html)

---

## 1. Who processes your data

**Maxime Bouchard**, acting as an individual, publisher of the KiFéKoi app.

For any question, or to exercise your rights:
[mbouchard.dev@gmail.com](mailto:mbouchard.dev@gmail.com)

---

## 2. The most important point: two modes, two answers

KiFéKoi works in two ways, and **the choice is yours**. It lives in
*Settings › Household storage*.

### "On this device" mode (the default)

**No data leaves your phone.** No online account, no server, no remote backup.
Tasks, history, check-in answers and scores stay in the app's own storage.

In this mode this policy has almost nothing to describe: there is no processing
on our side, because there is no transmission. The only consequence is that a
household lost with the phone is lost for good.

This is the mode that is **active by default**. The app never switches on its
own.

### "Shared" mode

You choose this mode to share a household across several devices. The data
described below is then hosted on a server.

---

## 3. Data processed in shared mode

| Data | Why | Legal basis (GDPR) |
|---|---|---|
| **First name** entered during onboarding | Identify who carries what | Performance of a contract (Art. 6(1)(b)) |
| **Anonymous account identifier** | Link your device to your seat in the household | Performance of a contract |
| **Household content**: tasks, notes, due dates, assignments, history | The service itself | Performance of a contract |
| **Weekly check-in answers** | Compare felt experience with the computed score | Performance of a contract |
| **Push notification token (APNs)** | Tell you when someone assigns you a task | **Consent** (Art. 6(1)(a)) |
| **Subscription transaction identifier** | Verify with Apple that the subscription is active | Performance of a contract |

### About the "anonymous" account

The account is created with no e-mail and no password: the app asks for a first
name and nothing else. The resulting identifier contains no information about you
and is linked to no directory.

One consequence worth knowing: **this account lives in your device's keychain**.
Losing it means losing access to the shared household, with no recovery path.

### About check-in answers

These are the most personal data in the app — people write things like "I felt
like I was the only one thinking about it". They are readable only by members of
your household. That restriction is not a promise on our part: it is enforced by
the database itself (*Row Level Security*), independently of the app's code.

### About the notification token

It is only transmitted if you turn remote notifications on, and it is deleted
from the server as soon as you turn them off. This is the only processing based
on your consent, and it is therefore revocable at any time, with no consequence
for the rest of the service.

---

## 4. What we do not do

- **No advertising.** The app embeds no ad network.
- **No tracking.** No analytics SDK, no advertising identifier, no audience
  measurement, no cross-app tracking. The privacy manifest shipped with the app
  declares `NSPrivacyTracking: false`.
- **No selling or commercial sharing.** Your data goes to no one other than the
  technical processors listed below.
- **No profiling and no automated decisions** producing legal effects concerning
  you. Balance scores are a displayed calculation, not a decision.
- **No reading by us.** The publisher does not access household content.

---

## 5. Processors

| Provider | Role | Location |
|---|---|---|
| **Supabase** | Database and server function hosting | **Ireland (European Union)** |
| **Apple** | Notifications (APNs), purchases and subscriptions | Per Apple's policy |

**Your household's content does not leave the European Union.** The database and
server functions are hosted in Ireland, so there is no transfer outside the EU to
document for that data.

Two caveats, stated plainly: notifications travel through Apple's servers (APNs)
and subscription verification queries the App Store. Both follow Apple's policy
rather than ours, and both carry only a device token and a transaction
identifier — never your household's content.

Apple is also the payment intermediary for subscriptions: **we neither receive
nor see any payment data**.

---

## 6. Retention

- **Household content**: kept for as long as the household exists. Deleted
  immediately and permanently when the last member leaves or deletes it.
- **Account**: deleted immediately on your request (see §8).
- **Notification token**: deleted as soon as notifications are turned off, or
  automatically when Apple tells us the app has been uninstalled.
- **Subscription record**: kept while the subscription runs, then marked as
  revoked so that we can answer "why did this go back to free?".

---

## 7. Your rights

You have the rights of access, rectification, erasure, restriction, objection and
portability provided by the GDPR, as well as the right to withdraw your consent
to notifications at any time.

Two of these can be exercised **directly in the app**, without writing to anyone:

- **Rectification**: *Settings › Members*, for the first name.
- **Erasure**: *Settings › Delete my account* (see §8).

For the others, write to the address in §1. You may also lodge a complaint with
your supervisory authority — in France, the [CNIL](https://www.cnil.fr).

---

## 8. Deleting your account

*Settings › Delete my account*, in the app.

Exactly what it does:

1. Your seat in the household is removed, along with your first name.
2. Your account is deleted from the authentication server.
3. Your notification tokens are deleted.
4. **If you were the last member**, the household and all its content are deleted
   with you.

What it does **not** do: if other people share the household, the household and
its history remain theirs. We do not destroy a third party's data because you are
leaving — but the occurrences you carried stop being attributed to you.

The operation is immediate and irreversible.

---

## 9. Security

- All communication goes over **HTTPS**.
- Separation between households is enforced by the database (*Row Level
  Security*), not by the app's code. A programming error in the app therefore
  cannot expose someone else's household.
- The server's administration key exists only on the server. It is **never**
  embedded in the app.

No system is impenetrable, and we do not claim otherwise.

---

## 10. Children

KiFéKoi is aimed at adults living in a household. The app is not directed at
children under 15 and does not offer them an account.

A household may nonetheless include members marked as "child". In that case,
**only their first name is recorded, by an adult of the household, and they have
neither an account nor access to the app**. It is for the adult who adds them to
make sure that this is appropriate.

---

## 11. Changes

Any change will be published on this page with a new update date. A substantial
change will be signalled inside the app.
