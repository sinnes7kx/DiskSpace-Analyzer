DISKSPACE ANALYZER 1.6.3 FREE - 16 November 2026
=============================================

NEW VERSION NOTIFICATIONS
The app now checks the official GitHub Releases feed on a background thread.
Automatic checks start after the interface is ready and run at most once daily.
A non-modal card announces a newer stable version without taking keyboard focus
or interrupting scans. View release opens the official page on an explicit click.
No automatic download or installation is performed.

Settings includes an automatic-notification switch and Check for updates button.
The Settings content scrolls so controls remain reachable on smaller screens.
Dismissed versions are remembered; a manual check can show the notice again.
Network failures do not open error dialogs. No scanned file information is sent.
Version tags compare numerically, so 1.6.10 correctly follows 1.6.9.

Retains all 1.6.2 fixes below. See VERIFICATION.md for checks and limitations.

DISKSPACE ANALYZER 1.6.2 FREE - 16 November 2026
=============================================

LAPTOP SIZING AND SORTING
Startup now fits the current monitor work area instead of requesting a fixed
1340x840 window. UI scale adapts when the minimum layout would exceed the screen.
Maximize converts physical monitor dimensions to CustomTkinter logical units,
leaving the taskbar area clear. Restore and dialogs are constrained to the work area.
Rows remain steady during scanning and sort once at completion, largest first by
default. A column sort chosen by the user is preserved.

LARGER TEXT AND LINKS
The former Larger text setting is now permanent. The size selector is removed,
and older saved Standard preferences no longer reduce detail/status text size.
Settings now includes GitHub (https://github.com/sinnes7kx) and an additional
Donate link. The existing rail Donate button and fixed PayPal URL are unchanged.

VALIDATE ONLINE
Validate opens a browser search directly, using only the selected item's name.
Its tooltip is exactly: Validate - Check online if it's safe to delete
Hovering and selecting rows do not send online requests.
Local review remains available via right-click > Review local Delete Check.
Online results are research, not a deletion-safety verdict. Deletion guards remain.

COHESIVE STARTUP
The root window remains hidden while controls are created. Layout, initial meters,
empty state and window integration are prepared at zero opacity, then the complete
window is revealed with one 180ms fade. Reduced motion reveals it immediately.
Native title-bar styling avoids nested update loops and hide/show transitions.
The application icon is present from the first frame, and a duplicate initial
disk-capacity query has been removed.
Name-column width is explicitly fitted on resize, avoiding an overflow exposed by
the earlier layout pass. No claim of a measured whole-program speedup is made.

RETAINED
All features remain free. Stable live row ordering, default Scan/Stop labels,
Windows Delete hiding, long-path support, bounded transient retries, partial-data
reporting, dark dialogs/menus, history, comparisons and exports remain included.

See VERIFICATION.md for measured checks and remaining Windows acceptance limits.
