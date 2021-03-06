---
-api-id: P:Windows.UI.StartScreen.SecondaryTile.LockScreenDisplayBadgeAndTileText
-api-type: winrt property
---

<!-- Property syntax
public bool LockScreenDisplayBadgeAndTileText { get;  set; }
-->

# Windows.UI.StartScreen.SecondaryTile.LockScreenDisplayBadgeAndTileText

## -description
Gets or sets whether the secondary tile is eligible to display both a badge and a detailed tile on the lock screen. If you set this property to **True**, you must also provide a badge image through the [LockScreenBadgeLogo](secondarytile_lockscreenbadgelogo.md) property. If you do not want to use the detailed tile capability, provide a badge image through the [LockScreenBadgeLogo](secondarytile_lockscreenbadgelogo.md) property and set [LockScreenDisplayBadgeAndTileText](secondarytile_lockscreendisplaybadgeandtiletext.md) to **False**.

> [!NOTE]
> Stating that your secondary tile is eligible for a lock screen presence does not guarantee that it will have one. Only the user can add an app to one of the seven lock screen slots, as well as choosing which one of them can display detailed tile information. For more information, see the [Lock screen overview](http://msdn.microsoft.com/library/07fefb48-f55c-4ab7-8b68-a8aed11074fd).

## -property-value
**True** if the secondary tile can have a lock screen presence; otherwise, **False**.

## -remarks

## -examples

## -see-also
[Secondary tiles overview](http://msdn.microsoft.com/library/973391ca-a4f1-40f7-a909-5396b4a2bd18), [Lock screen overview](http://msdn.microsoft.com/library/07fefb48-f55c-4ab7-8b68-a8aed11074fd), [Secondary tiles sample](http://go.microsoft.com/fwlink/p/?linkid=231487), [Lock screen app sample](http://go.microsoft.com/fwlink/p/?linkid=239970), [Guidelines and checklist for secondary tiles](XREF:TODO:m_ui_tiles.guidelines_and_checklist_for_secondary_tiles), [Guidelines and checklist for tiles and badges](http://msdn.microsoft.com/library/e825f754-97dd-41c2-aff4-4dfb60eda677), [Quickstart: Showing tile and badge updates on the lock screen](XREF:TODO:m_ui_tiles.howto_optin_for_lockscreen), [How to send notifications to a secondary tile](XREF:TODO:m_ui_tiles.howto_send_notifications_to_secondary_tiles), [Quickstart: Pinning a secondary tile](XREF:TODO:m_ui_tiles.quickstart_creating_secondary_tile), [Pinning secondary tiles](http://msdn.microsoft.com/library/54a4d4d3-0430-45eb-b5fd-ee96598c216e)