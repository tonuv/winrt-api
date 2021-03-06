---
-api-id: M:Windows.UI.Notifications.BadgeUpdater.StartPeriodicUpdate(Windows.Foundation.Uri,Windows.Foundation.DateTime,Windows.UI.Notifications.PeriodicUpdateRecurrence)
-api-type: winrt method
---

<!-- Method syntax
public void StartPeriodicUpdate(Windows.Foundation.Uri badgeContent, Windows.Foundation.DateTime startTime, Windows.UI.Notifications.PeriodicUpdateRecurrence requestedInterval)
-->

# Windows.UI.Notifications.BadgeUpdater.StartPeriodicUpdate

## -description
Begins a series of timed updates for the badge from a web resource that the updater is bound to. Updates begin at a specified time. Note that only web resources (http/https) are allowed in a periodic update.
<!-- @WRITER erictill 1/13/2012 : Nathan wants the following added, but I have no idea what he's talking about. Wrote him. : Only one periodic update can occur for each tile (per type). -->

## -parameters
### -param badgeContent
The Uniform Resource Identifier (URI) from which the XML content of the badge update will be retrieved.

### -param startTime
The time at which the Uniform Resource Identifier (URI) should first be polled for new badge content.

### -param requestedInterval
The frequency with which the Uniform Resource Identifier (URI) is polled for new badge content, following the initial update at *startTime*.

## -remarks

## -examples

## -see-also
[StartPeriodicUpdate(Uri, PeriodicUpdateRecurrence)](badgeupdater_startperiodicupdate_1967457783.md), [App tiles and badges sample](http://go.microsoft.com/fwlink/p/?linkid=231469), [Guidelines and checklist for tiles and badges](http://msdn.microsoft.com/library/e825f754-97dd-41c2-aff4-4dfb60eda677), [How to clear a badge](XREF:TODO:m_ui_tiles.howto_clear_a_badge), [How to send a glyph or numeric badge in a local notification](XREF:TODO:m_ui_tiles.howto_send_local_badge_notifications), [How to set up periodic notifications for badges](XREF:TODO:m_ui_tiles.howto_setup_badge_polling), [How to update a badge through push notifications](XREF:TODO:m_ui_tiles.howto_update_badges_push), [Badge XML schema](XREF:TODO:badge.Schema_Root), [Badge overview](http://msdn.microsoft.com/library/a64c58bb-d9c9-4c09-a685-4df94fa7dfdd)