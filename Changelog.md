# CoFrance v2.1.5 Changelog

### Improvements
- Further improvements on tag Anti-Overlap
- REL notification now auto acknowledge 10 seconds after accepted transfer

### Additions

### Fixes
- Fixed AFK tag field tooltip not resetting
- Fixed Assigned squawk format issue when empty
- Fixed Joystick buttons making modifier key stuck
- Fixed Popup open positions to work on secondary screens
- Fixed SHRQ remaining on tag once transfer accepted
- Fixed Flight Group Filter window closed state not saved


# CoFrance v2.1.4 Changelog

### Improvements
- Improved minimized tag placement
- Improved Tag Anti-overlap
- Window position & visibility now reloaded when switching settings

### Additions
- Added persistence to Flight Group Filter window position/state

### Fixes
- Fixed Side Menu window not opening correctly if side menu on 2nd screen
- Fixed lists not opening correctly on 2nd screen


# CoFrance v2.1.3 Changelog

### Fixes
- Recompiled Binary


# CoFrance v2.1.2 Changelog

### Improvements
- Increased Radar pointer safety

### Additions
- Added `.ring <position>` command

### Fixes
- Fixed Datablock icon using wrong font if flight was unconcerned
- Fixed Sector Indicator showing current owning sector if flight was Unconcerned
- Fixed Find command showing wrong position when element not found
- Fixed Man Trf popup sector ordering
- Fixed OBS and SUP being displayed in Man Trf popup
- Fixed unseen TRANSFER IN flights displayed in regular font
- Fixed TCT update not triggered when switching to TCT enabled profile
- Fixed Range Rings side menu button state not updated when switching Radar Screen


# CoFrance v2.1.0 Changelog

### Improvements
- Removed persistence logs
- Using private font loading instead of system wide fonts

### Additions
- Added Assign Current ("CURR") button inside ASSR popup
- Added Auto-Updater
- Added `.cofrance report` & `.cofrance changelog` commands
- Added CoFrance Window Hide side menu button

### Fixes
- Fixed Hand-off tag minimization position
- Fixed asr data saving on non-CoFrance Radars
- Fixed issue with notified flights not starting as not seen
- Fixed heavy lags when dragging tags with Dynamic DyP opened
- Fixed Agenda & DyP not hiding on non-CoFrance radar screen
- Fixed Inset Radar Window 2 named "Inset 1" in window header
- Fixed CoFrance Window Display Window incorrect opened state
- Fixed Contactme being available on assumed aircraft instead of Transfer In aircrafts
- Fixed Contextual filter blinking when using CTRL as modifier key
- Removed predicted EOD/TOD/TOC/EOC


# CoFrance v2.0.8 Changelog

### Improvements
- Flights Lists are now togglable inside CoFrance Window Display Window instead of Radar Menu
- Right Click on scratchpad clears it
- Can't input more than 4 char inside ASSR popup text entry
- Popups now only accepts numeric inputs
- Keyboard entry box now behave like native OS input box
- Right Click on a predefined view now save current viewing area to selected view
- Adjusted Zoom button increment
- Static STCA (STCA between unconcerned/notified flights) are now filterable
- CoFrance Windows now hide instantaneously when switching to non-CoFrance radar screen

### Additions
- Added Drag heading in Inset Radar Window
- Added Radar Menu and Track Menu actions to Inset Radar Window
- Added Custom Area Filters
- Added Setting Profiles selection
- Added per ASR Setting Profile
- Added Contact Me button to callsign menu of "tracked by other" flights

### Fixes
- Fixed TOD/BOC/EOC/EOD predictions not cleaned up
- Fixed agenda not updated immediately when adding datablock
- Fixed ° char in QDM/SEP
- Fixed Drag heading assigning 000 instead of 360
- Fixed ALTGR triggering modifier action after being released
- Fixed Find command timer starting even if not on CoFrance Radar screen
- Fixed inset not using associated radar's tag format
- Fixed flights disappearing randomly on inset window
- Fixed Auto Flight Leg remaining drawn after acknowledging flight
- Fixed auto flight leg/temporary flight leg delay before hiding


# CoFrance v2.0.7 Changelog

### Improvements
- Renamed Man Trf UNICOM to ADVISORY
- Adjusted history trail and track symbols sizes
- Restricted CPDLC connection to CTR positions
- Inbound SHRQ now triggers Find on concerned flight
- Inbound SHRQ notification now takes highest priority

### Additions
- Added Striped list option
- Added 6, 7, 8, 9, 12 nm interring distance for Range Rings
- Added Ground State popup
- Added Views management window
- Added Inset Windows
- Added Static & Dynamic DyP windows
- Added temporary Route draw
- Added TOD/BOC/EOD/EOC predictions drawing on route
- Added CoFrance Windows Display window

### Fixes
- Fixed z-order drawing of lists contextual menu
- Fixed z-order drawing of side menu windows
- Fixed List entry drawing not being vertically centered
- Fixed List Header not being vertically centered
- Fixed min/max speed character
- Fixed Holding list holding indicator character
- Fixed CoFrance windows visible on non-CoFrance ASRs
- Fixed AFL displaying Pressure Altitude instead of Fight Level
- Fixed default Group Highlight symbol
- Fixed Datablock symbol
- Fixed ° char in QDM Drawing
- Fixed FPASD symbol not being aligned with aircraft heading
- Fixed squawk 7400 notification tooltip


# CoFrance v2.0.6 Changelog

### Improvements
- Improved leader line drawing
- Clicking primary track symbol can now be used to send Euroscope commands
- Left Click on Speed Vector Side Menu button now toggle speed vector
- Multiline Text Input box support
- Switched to using only one font (`CoFrance.ttc`)

### Additions
- Added auto CPDLC removal of messages in CPDLC message list (10mins)
- Added CPDLC rectangle around Assigned squawk
- Added CPDLC LOGOFF message to message list
- Added custom Text input boxes
- Added Text Entry field inside ASSR Popup
- Added OAT & GAT route switch point
- Added STAY notification

### Fixes
- Readded scrolling speed vector button to cycle speed vector value
- Fixed Hover QDM target selection triggering Speed Vector control
- Fixed Hover QDM target selection not saved throughout draw calls
- Fixed popups having window framing when they should not
- Fixed List context menu opening on uncompatible lists
- Fixed stale CPDLC list entry when flight disconnect
- Fixed Streamdeck speed vector controls
- Fixed Text input boxes not being drawn
- Fixed AFL rounding
- Fixed CR contextual filter
- Fixed blinking departure list

### Note
- Disabled Alert List until update


# CoFrance v2.0.5 Changelog

### Improvements
- Improved all window rendering to use layered windows
- Improved backend window management
- Speed vectors are now ASR dependant
- Adjusted minimized tag position
- Improved Leader Line drawing
- POINT now uses Coordination Tag field instead of Notification
- Increased refresh rate of Coordination Tag field
- Hovering single aircraft QDM info box now shows same information as in preview mode

### Additions
- Added turn radius when dragging Heading
- Added Not Seen list
- Added Negotiation list
- Added FL? point symbol
- Added Abbreviated Flight Plan Creation window

### Fixes
- Fixed Virtual Machine file path not being parsed correctly
- Fixed text-only message not prefiling
- Fixed incorrect ground speed formatting for speed inferior to 100kts
- Fixed incorrect ordering in SCH list of man trf popup
- Fixed CFL contextual filter being too restrictive
- Fixed group highlight and invidualVV not forcing speed vector drawing if disabled
- Fixed CPDLC uplink canceling on CFL, AHDG, WAYPOINT
- Fixed empty line between tag and CPDLC request
- Fixed CLAM showing if no CFL set
- Fixed AFL being rounded down
- Fixed CR tooltip not deleted
- Fixed UNICOM not showing in Man Trf window
- Fixed no FP flight being filtered
- Fixed Point Popup opening position
- Fixed RAM Alert triggering when flight was in a turn
- Fixed Right Click on callsign intercepted by drawn route below when trying to mark flight as seen
- Fixed ASPD CPDLC message


# CoFrance v2.0.3 Changelog

### Additions
- Added clearer information on "Add Departure List" window
- Quick QDM now uses Double `Modifier + Left Click`
- Added ASSR popup

### Fixes
- Fixed UNICOM not being available inside Man Trf scheduled list if not empty
- Fixed Man Trf always sending as CPDLC disregarding DLK button state
- Fixed `Alt + Left Click` on SI not sending CPDLC handoff
- Fixed De-Assume always sending CPDLC handoff
- Fixed CPDLC history message window now scroll to the end automatically
- Fixed STCA warning concerned flights being added to alert list
- Fixed RAM displaying when cleared Approach
- Fixed Holding lists opening when hold assigned to not Assumed traffic
- Fixed `Alt + Left Click` not sending ASSR via CPDLC


# CoFrance v2.0.2 Changelog

## Additions
- Added route preview when hovering COPN/COPX popups
- Manual Transfer popup now opens centered and on a non empty list if available
- Added custom RAM and CLAM computations
- Complete Route now displays when extrapolating
- Added auto mouse cursor positioning option
- Transfer Confirmation window now moves cursor to transfer button if option is enabled
- Find window now auto focuses entry field when opening and moves cursor to it if option enabled
- Now saving Agenda window size & position
- Minimizing tag now moves them close to track symbol
- Added SID & ARWY in intention field for approach positions
- Added Quick QDM using `double Left Click` on radar background *(Now, to close a chat window, use `double Right Click` instead of `double Left Click`)*
- Added UNICOM option in Manual Transfer popup to allow `double Left Click` Sector Indicator to release a flight
- Added RNAV capabilities inside INFO tab of Extended Tag

## Fixes
- Fixed list menu being mapped to `Modifier Right Click` instead of `Modifier Left Click`
- Fixed opening CCAMS squawk menu being bound to `Right Click` instead of `Left Click`
- Lost aircraft (GHOST) track symbol changed to FPASD
- Fixed acknowledging of Lost flight in Lost List not removing flight from list
- Improved History Trails lines drawing
- Fixed ASSR, RAM, CLAM, AFK notifications not showing again after being manually cleared
- Fixed Tag Formats not updating when changing runway config
- Fixed Tag Format "flightstate" property parsing
- Fixed config files auto downlaod
- Removed unused and confusing "airway_filepath" property inside CoFrance_Preference.toml
- Fixed Euroscope UI disappearing due to DC corruption
- Fixed unconcerned flight not showing correctly in Alert List
- Fixed track symbol size and drawing
- Fixed horizontal Side Menu panel display
- Fixed route not updating with flight progression
- Fixed STCA not updating after conflict has passed
- Fixed route deviation when a Direct-To was assigned
- Fixed Alert List not being cleared when deactivating STCA
- Fixed DLK button not being enabled in Manual Transfer popup
- Fixed unconcerned STCA being added to Alert List
- Fixed Contact Me & CPDLC flag disappearing
- Fixed Text Only message pre-filing
- Fixed Extended Tab font weight not updating correctly
- Fixed TCT not updating if both aircraft became unconcerned
- Fixed ASR setting not being saved correctly on close
- Fixed coordination popups UI drawing
- Fixed Euroscope windows (FP, runway configs,...) unable to open
- Fixed CPDLC Messages window not being ordered