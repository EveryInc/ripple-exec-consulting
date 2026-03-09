# Shareholder Email List Manager

## Prompt

I'm Chief Legal Officer at Ripple. Managing our shareholder communication lists is a surprisingly time-consuming task. Shareholders have multiple email contacts, people join and leave firms, we need different lists for different communication types (legal notices vs. quarterly updates vs. board materials), and changes need to be tracked for compliance.

Using the attached `shareholder_contacts.csv`, build me a tool that:

1. **Contact Database View** (interactive HTML)
   - Sortable/filterable table of all shareholders with: entity name, shareholder type (institutional, individual, board, strategic partner), primary contact, all email addresses, communication preferences, shares held, and status (active/inactive)
   - Support for multi-email shareholders (some entities have 3-4 different contacts who need different communications)
   - Search by name, email, entity, or shareholder type

2. **Distribution List Generator** - Generate clean email lists for different purposes:
   - **All Shareholders** - every active shareholder, primary contact only
   - **Quarterly Update Recipients** - shareholders who opted into quarterly updates (may include multiple contacts per entity)
   - **Legal Notices** - registered agents and legal contacts only
   - **Board Materials** - board members and board observers only
   - **Investor Relations** - IR contacts at institutional investors
   - Export each list as a comma-separated email string I can paste into Gmail BCC

3. **Change Management** - Show a log of all changes:
   - New shareholders added
   - Shareholders removed (and reason: sold shares, entity dissolved, etc.)
   - Contact information updates
   - Communication preference changes
   - Flag any shareholder whose contact info hasn't been verified in 6+ months

4. **Validation** - Check for:
   - Duplicate email addresses
   - Invalid email format
   - Shareholders with no primary contact assigned
   - Entities with outdated contact info (last verified > 6 months ago)

Output as a single interactive HTML file. Should feel like a simple CRM for shareholder communications.
