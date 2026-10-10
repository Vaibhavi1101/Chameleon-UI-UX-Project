# Adaptive Color — Design Documentation

## 1. Purpose
This module demonstrates two color presentations of the Chameleon analytics dashboard: a light **Normal Color State** and a dark **Adaptive Color State**.

## 2. Included UI States
### Normal Color State
- Dark navy header and sidebar.
- Pale blue-gray main canvas.
- White dashboard cards.
- Dark text on light surfaces.
- Blue chart marks and green/yellow status indicators.

### Adaptive Color State
- Dark navy header and sidebar.
- Near-black main canvas.
- Dark navy dashboard cards.
- Light text on dark surfaces.
- Blue chart marks and light blue bars.
- Green/yellow status indicators retained.

## 3. Shared Components
Both states retain the same main dashboard components:
- Overview heading and date-range selector.
- Total Revenue, Total Orders, and Active Customers KPI cards.
- Sales Performance chart.
- Recent Activity card.
- Recent Transactions table.
- Sidebar navigation and top navigation controls.

The layout and information structure remain substantially consistent so the main change is the color presentation.

## 4. Intended Adaptive Behavior
The design proposes changing the dashboard from the light state to the dark state when an alternate visual presentation is appropriate for the user context.

**Important implementation note:** The supplied screens show the visual states only. They do not demonstrate a working ambient-light sensor, automatic state switching, or an implemented APCA calculation. Do not describe those mechanisms as completed functionality unless separately implemented and verified.

## 5. Design Rules
- Keep layout, spacing, and component structure consistent between states.
- Use light text on dark surfaces and dark text on light surfaces.
- Preserve recognizable chart colors and status indicators.
- Check contrast for primary text, secondary labels, table content, chart axes, and status badges.
- Do not rely on color alone for status communication.
- Verify that muted text remains readable in both states.

## 6. Validation Checklist
- [ ] Compare text legibility in both states.
- [ ] Check contrast of headings, body text, and muted labels.
- [ ] Check chart line, bars, axes, and labels in both states.
- [ ] Check Completed and Pending status badges in both states.
- [ ] Confirm the same data and sections appear in both states.
- [ ] Test the transition or state selection if a prototype interaction is available.
- [ ] Record any contrast calculations or user-test findings separately; none were provided with the supplied screenshots.

## 7. Current Status
**Demonstrated:** two designed dashboard color states, with a largely consistent layout and content structure.

**Not established by the supplied screens:** real-time ambient-light sensing, automatic color adaptation, APCA-based calculations, production implementation, or user-testing outcomes.

## 8. Files / Evidence
Add the relevant Figma link and screenshots of both states when integrating this document into the repository.

- Normal Color State: `Normal Color State.png`
- Adaptive Color State: `Adaptive Color State.png`
