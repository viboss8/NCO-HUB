# NCO Mission Control, Fictional Public Demo

This is a browser-only static prototype using **fictional names, assignments, course records, deadlines, and other demo data**. It is **not authorized for real Army personnel information**. Never enter real Soldier records, appointment details, packets, medical information, or sensitive mission data.

## Preview and deployment

1. Create a **new, separate repository**, e.g. `nco-mission-control-demo`. Do not use your personal `mission-control` repository.
2. Upload both `index.html` and `README.md` to the repository root.
3. To publish this strictly fictional demo with GitHub Pages, open repository **Settings > Pages > Build and deployment > Deploy from a branch**, select **main** and **/(root)**, then save. Pages will display a website address when deployed. Public Pages websites are viewable by others.
4. In later edits, push changes to the same repository, and Pages will update at the same URL.

## Data warning

The site stores demo edits in browser localStorage, meaning data **does not synchronize across devices**, may be lost if browser storage is cleared, and **should not be used for real records**. Even a private repository does not make its public Pages site private. Obtain authorization and appropriate secured Army/DoD storage before using actual personnel or operational information.
## Mobile-first update

The interface is optimized for phone screens, including 44px minimum tap targets, readable 16px form inputs, and a full-width mobile editing drawer. The guided setup was checked at 375px and 390px screen widths. Only fictional examples may be entered into this public demo.

## Working-day deadlines and calendar

The preparation wizard offers 1 to 10 working days before the event, plus a custom deadline. Calculated dates skip Saturdays, Sundays and OPM observed federal holidays. It also skips the specifically published JBLM DONSAs currently listed in the demo (Nov 27, Dec 24 and Dec 31, 2026; Jan 15, Feb 12 and May 28, 2027). These local dates are not an authoritative schedule for the user's unit. Verify applicability and update as more dates become available. Sources: https://www.opm.gov/policy-data-oversight/pay-leave/federal-holidays/ and https://home.army.mil/lewis-mcchord/.

Custom dates remain user-selected. Calculations do not create verified completion or attendance and do not make the app suitable for real personnel data.


## Mobile tracker release (November 2026)
- Starts with a blank roster instead of fictional preloaded records.
- Add/edit Soldiers by rank and last name, optional first name and role, with linked appointments, training requirements, and follow-ups.
- New calendar events default to generic "Appointment"; do not add medical reasons.
- Home has quick actions for follow-ups, appointments, and event preparation.
- A new browser storage key protects older prototype data from accidental overwriting.
- Optional passphrase mode uses Web Crypto AES-256-GCM, PBKDF2-SHA256 (250,000 iterations) with random salt/IV per encrypted save.
- Encryption setup migrates current local tracker data and removes the current unencrypted storage key upon successful encryption.
- Download and restore the encrypted JSON backup. Protect the passphrase; there is no recovery service.
- Test coverage included JavaScript parse checks and simulated UI flows for adding a Soldier, appointment, task, and locking/unlocking saved records. This is not a substitute for device/browser acceptance testing.

**Important:** This is public static website code. Browser data is not automatically uploaded to the GitHub repository, synchronized, or backed up. Local encryption protects stored data at rest but does not secure a compromised browser or make the site an Army-authorized system. Do not store personnel schedules or nonpublic work records without confirmation of the approved environment.
