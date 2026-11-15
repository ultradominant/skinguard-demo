# SkinGuard — functional browser MVP for examiners

This is an **additional browser-accessible demonstration** of the supplied SwiftUI MVP's **simulated business rules**. It is not a live payment system. The original iPhone app archive remains a separate source artifact.

## Open it

Open `index.html` in a modern browser. No dependencies, build process, server, login or internet connection are required for the basic demonstration. The app stores fictional local state in the current browser using `localStorage`; use **Reset demo** to return to the starting conditions. It can also be hosted as static files on GitHub Pages; upload `index.html`, `styles.css`, and `app.js` to the root of a public repository and enable GitHub Pages.

## Demonstrate real functionality

1. In **Child space**, choose Yermek. Select **Make a payment** → **Orbit Quest**.
2. The app shows the game-purchase parental approval requirement. Click **Ask a parent**. The balance should remain at 45,500 KZT.
3. Switch to **Parent**. Find the pending request and **Approve demo payment**. The Yermek balance becomes **40,600 KZT**, and another approval is impossible.
4. In **Activity**, verify the Paid record. Change to Islam and confirm his independent balance is unchanged.
5. Use **Learn** to complete the first safety lesson. The selected child's local progress and XP update.
6. Press **Reset demo** before another demonstration.

The original SwiftUI iPhone source is in the supplied ZIP. This web version intentionally mirrors rule logic but is not generated from the SwiftUI source, is not bank-integrated and has not been subject to penetration testing. Do not enter personal or real banking data.

## Important disclaimers

All seller labels and transactions are simulated; selecting Parent is a UX demonstration, not secure authentication. The webpage cannot intercept real payments or control other apps, and its data in localStorage is suitable only for non-sensitive demo records. Five real user-test sessions and a user-driven improvement are still required for the final rubric.

## QA change, 13 November 2026
An explicit confirmation now precedes fictional parent approval. Cancel leaves the request pending and balance unchanged. This was a developer/automated QA refinement, NOT a change proven by five external usability participants. The 10-case Chromium test log is in the separate evidence appendix and final package.
