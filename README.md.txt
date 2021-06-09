# Creating a skin:

A `skin.xml` file is read by the GUI Skin (CImageGUISkin). The order of elements/groups does not matter and they are not case sensitive.

* Create a folder inside the `skin` folder with your skin name.
* Add to that folder a `skin.xml` file.
	* Optionally, also add a `textures` folder inside the `skin` folder. If any files are added to it, the skin will apply those to overridde the default ones in the game's main `textures` folder.

At the end of this file you have a **template**.


# Groups availables:
	* Properties: contains information about the current skin file.
	* Global: contains elements that change the global enviroment
	* Custom: contains elements, all optional, that change specific parts of the GUI.


## Properties
Elements here are all optional.

* Author
* Version
* Date
* Desc
* Fallback
* Font


## Global
Elements here change the colors in the multiple areas in the game.

* EGDC_3D_DARK_SHADOW : Dark shadow for three-dimensional display elements.
* EGDC_3D_SHADOW : Shadow color for three-dimensional display elements (for edges facing away from the light source).
* EGDC_3D_FACE : Face color for three-dimensional display elements and for dialog box backgrounds.
* EGDC_3D_HIGH_LIGHT : Highlight color for three-dimensional display elements (for edges facing the light source.) Changes the color used as background in dropdown menus like the banlist selection one and the deck selection dropdown
* EGDC_3D_LIGHT : Light color for three-dimensional display elements (for edges facing the light source.)
* EGDC_ACTIVE_BORDER : Active window border.
* EGDC_ACTIVE_CAPTION : Active window title bar text. Changes the color of the text used for the version name and/or title of menus, WHILE they are enabled.
* EGDC_APP_WORKSPACE : Background color of multiple document interface (MDI) applications.
* EGDC_BUTTON_TEXT : Text on a button. Changes the color of the text used in buttons. Also change the color of the text displayed in "Card Info"
* EGDC_GRAY_TEXT : Grayed (disabled) text. Changes the color of the text used in box that are "grey", usually. Examples: the phase buttons when pressed, the thext in the "Attribute" and "type" menus, while the "monster" category is not selected
* EGDC_HIGH_LIGHT : Item(s) selected in a control. Changes the color used as highlight/background for the item you are currently seeing in a drop down selection menu, like the banlist.
* EGDC_HIGH_LIGHT_TEXT : Text of item(s) selected in a control. Changes the color of the text used in the main screen's top left menus
* EGDC_INACTIVE_BORDER : Inactive window border. Changes the color used for the retangular area where the version name in the main screen's menu is placed.
* EGDC_INACTIVE_CAPTION : Inactive window caption. Changes the color of the text used in for the version name and/or title of menus, WHILE they are disabled test changing it, then go to the main menu and click in a free are, so the menu becomes "inactive" 
* EGDC_TOOLTIP : Tool tip text color
* EGDC_TOOLTIP_BACKGROUND : Tool tip background color
* EGDC_SCROLLBAR : Scrollbar gray area. Changes the color of the scroll bar used in Deck edit's search results.
* EGDC_WINDOW : Window background
* EGDC_WINDOW_SYMBOL : Window symbols like on close buttons, scroll bars and check boxes. Changes the color 'arrows' used in the deck selection dropdown menu and the arrows used when you need to scroll to see more results for something in a selection
* EGDC_ICON : Icons in a list or tree
* EGDC_ICON_HIGH_LIGHT : Selected icons in a list or tree
* EGDC_GRAY_WINDOW_SYMBOL : Grayed (disabled) window symbols like on close buttons, scroll bars and check boxes. Changes the color for the arrows in dropdown menus.
* EGDC_EDITABLE : Window background for editable field (editbox, checkbox-field). Changes the color for the search boxes while they are available to accept text
* EGDC_GRAY_EDITABLE : Grayed (disabled) window background for editable field (editbox, checkbox-field).  Changes the color for the search boxes while they are disabled
* EGDC_FOCUSED_EDITABLE : Show focus of window background for editable field (editbox or when checkbox-field is pressed). Changes the color for the search boxes when they are enabled [when you click on them]
* CheckBoxColor : Changes the color used for the check markers in the checkboxes, like the "Show unofficial card"
* Caption : takes tbardistancex and tbardistancey : Changes the coordinates used for the text in the Version name, Update Log, etc
* WindowButton : takes a width: Changes the width in the'arrows' used in the deck selection dropdown menu, category dropdown menu, etc


## Custom

* CARDINFO_IMAGE_BACKGROUND : Changes the color used as background for the area where the card picture is displayed in Deck Edit
* CARDINFO_ARCHETYPE_TEXT_COLOR : Changes the color used for the archtypes names in the card details area
* CARDINFO_STATS_COLOR : Changes the color used for the Archetype Name in the "Card Info" area
* CARDINFO_TYPES_COLOR : Changes the color used for the text with the types (Card Type, Attribute, monster type) in the "Card Info" area
* CARDINFO_PASSCODE_SCOPE_TEXT_COLOR : Changes the color used for the text with the the passcode and scope of a card in the "Card Info" area
* FPS_TEXT_COLOR : Changes the color used for the FPS displayed ingame
* DUELFIELD_ANNOUNCE_TEXT_BACKGROUND_COLOR
* DUELFIELD_ANNOUNCE_TEXT_COLOR : Changes the color used in the box after a card is announced. Example: Psi-Blocker
* DUELFIELD_CARD_OPPONENT_WINDOW_BACKGROUND : Changes the color for area around the caption text when you are selecting cards from a group. Example: when you are selecting what monsters to banish by Block Dragon.
* DUELFIELD_CARD_SELECTED_WINDOW_BACKGROUND : Changes the color for area around the areas like where the numbering for Extra Deck cards are, when you scroll through your Extra deck.
* DUELFIELD_CARD_SELECT_WINDOW_OVERLAY_TEXT
* DUELFIELD_CARD_SELECT_WINDOW_SET_TEXT : Changes the color for the caption text when you have to select cards from a location. Example: the Deck[1], Deck[2], etc, positions shown when you select a card with something like Terraforming
* DUELFIELD_CARD_SELF_WINDOW_BACKGROUND
* DUELFIELD_DISABLED_FIELD_COLOR
* DUELFIELD_HIGHLIGHTING_CARD_OUTLINE : Changes the color for the borders of a card, when it is selected. Example: a card that you add to your hand via Terraforming.
* DUELFIELD_HOVERED : Changes the color for the zone highlighted when you are hovering on the field.
* DUELFIELD_LINKED : Changes the color for the zones where a link monster points to.
* DUELFIELD_LP_1 : changes the color used for the value in your LP 
* DUELFIELD_LP_2 : changes the color used for the value in your opponent's LP 
* DUELFIELD_MUTUAL_LINKED : Changes the color for the zones where monsters co-linked with the monster that you hover the mouse over are.
* DUELFIELD_SELECTABLE_CARD_OUTLINE : Changes the color for the borders of a card, when it is selectable. Example: a Maxx C in your hand will have this color when asking you to activate it
* DUELFIELD_SELECTABLE_FIELD_OUTLINE : Changes the color for the borders of a zone , when you have to select it. Example: when selecting a zone to normal summon
* DUELFIELD_STACK: changes the color used for number in piles on the field, like the number of cards in a player's deck or extra deck.
* DUELFIELD_TOOLTIP_TEXT_BACKGROUND_COLOR : Changes the color used in the area for the tooltip box, the area with the card details when you hover the mouse over it on the field
* DUELFIELD_TOOLTIP_TEXT_COLOR:  Changes the color used in the text with the tooltip box.
* DUELFIELD_TURN_COUNT : the color used the for the turn count
* DUELFIELD_TURNPLAYER_COLOR: the color used for the area where the LP bar, player name and timer are drawn.
* DUELFIELD_TURNPLAYER_OUTLINE_COLOR: the color around the area where the LP bar, player name and timer are drawn.
* PROGRESSBAR_FILL_COLOR : Changes the color used for the elapsed progress bar in repositories. 
* PROGRESSBAR_EMPTY_COLOR : Changes the color for remaining progress bar for repositories
* ROOMLIST_CUSTOM_ROOM : Changes the color for a room that has any of its settings changed from the default ones. Example: different LP, different starting hand, etc
* ROOMLIST_NORMAL_ROOM : Changes the color for a room that didn't have any of its settings changed from the default ones
* ROOMLIST_STARTED_ROOM : Changes the color for a room, in the room list, that has already started its duel.
* ROOMLIST_TEXTS_COLOR : Changes the color for the texts in the room list menu. Examples: the "Server", "Nickname", "show locked rooms" texts
* The following 41 fields change the color used for the areas in Deck Edit, specifically for the areas where the informations about the deck are displayed. Example, the panel where you see `Monsters 32, Spells 5, Traps 3`.
	* DECK_WINDOW_EXTRA_INFO_BOTTOM_LEFT
	* DECK_WINDOW_EXTRA_INFO_BOTTOM_RIGHT
	* DECK_WINDOW_EXTRA_INFO_TOP_LEFT
	* DECK_WINDOW_EXTRA_INFO_TOP_RIGHT
	* DECK_WINDOW_EXTRA_INFO_OUTLINE
	* DECK_WINDOW_EXTRA_BOTTOM_LEFT
	* DECK_WINDOW_EXTRA_BOTTOM_RIGHT
	* DECK_WINDOW_EXTRA_TOP_LEFT
	* DECK_WINDOW_EXTRA_TOP_RIGHT
	* DECK_WINDOW_EXTRA_OUTLINE
	* DECK_WINDOW_HOVERED_CARD_RESULT
	* DECK_WINDOW_MAIN_INFO_BOTTOM_LEFT
	* DECK_WINDOW_MAIN_INFO_BOTTOM_RIGHT
	* DECK_WINDOW_MAIN_INFO_TOP_LEFT
	* DECK_WINDOW_MAIN_INFO_TOP_RIGHT
	* DECK_WINDOW_MAIN_INFO_OUTLINE
	* DECK_WINDOW_MAIN_BOTTOM_LEFT
	* DECK_WINDOW_MAIN_BOTTOM_RIGHT
	* DECK_WINDOW_MAIN_TOP_LEFT
	* DECK_WINDOW_MAIN_TOP_RIGHT
	* DECK_WINDOW_MAIN_OUTLINE
	* DECK_WINDOW_SEARCH_RESULT_INFO_BOTTOM_LEFT
	* DECK_WINDOW_SEARCH_RESULT_INFO_BOTTOM_RIGHT
	* DECK_WINDOW_SEARCH_RESULT_INFO_TOP_LEFT
	* DECK_WINDOW_SEARCH_RESULT_INFO_TOP_RIGHT
	* DECK_WINDOW_SEARCH_RESULT_INFO_OUTLINE
	* DECK_WINDOW_SEARCH_RESULT_BOTTOM_LEFT
	* DECK_WINDOW_SEARCH_RESULT_BOTTOM_RIGHT
	* DECK_WINDOW_SEARCH_RESULT_TOP_LEFT
	* DECK_WINDOW_SEARCH_RESULT_TOP_RIGHT
	* DECK_WINDOW_SEARCH_RESULT_OUTLINE
	* DECK_WINDOW_SIDE_INFO_BOTTOM_LEFT
	* DECK_WINDOW_SIDE_INFO_BOTTOM_RIGHT
	* DECK_WINDOW_SIDE_INFO_TOP_LEFT
	* DECK_WINDOW_SIDE_INFO_TOP_RIGHT
	* DECK_WINDOW_SIDE_INFO_OUTLINE
	* DECK_WINDOW_SIDE_BOTTOM_LEFT
	* DECK_WINDOW_SIDE_BOTTOM_RIGHT
	* DECK_WINDOW_SIDE_TOP_LEFT
	* DECK_WINDOW_SIDE_TOP_RIGHT
	* DECK_WINDOW_SIDE_OUTLINE
	* DECK_WINDOW_HOVERED_CARD_OUTLINE
* The following 8 fields change the color of the LP bar: LPBAR_1 (home), LPBAR_2 (away)
	* LPBAR_1_BOTTOM_LEFT
	* LPBAR_1_BOTTOM_RIGHT
	* LPBAR_1_TOP_LEFT
	* LPBAR_1_TOP_RIGHT
	* LPBAR_2_BOTTOM_LEFT
	* LPBAR_2_BOTTOM_RIGHT
	* LPBAR_2_TOP_LEFT
	* LPBAR_2_TOP_RIGHT
* The following 10 fields change the color of the timer: TIMEBAR_1 (home), TIMEBAR_2 (away)
	* TIMEBAR_1_BOTTOM_LEFT
	* TIMEBAR_1_BOTTOM_RIGHT
	* TIMEBAR_1_TOP_LEFT
	* TIMEBAR_1_TOP_RIGHT
	* TIMEBAR_1_OUTLINE
	* TIMEBAR_2_BOTTOM_LEFT
	* TIMEBAR_2_BOTTOM_RIGHT
	* TIMEBAR_2_TOP_LEFT
	* TIMEBAR_2_TOP_RIGHT
	* TIMEBAR_2_OUTLINE
* The following 12 fields change the color of card properties on the field
	* DUELFIELD_CARD_LEVEL
	* DUELFIELD_CARD_TUNER_LEVEL
	* DUELFIELD_CARD_RANK
	* DUELFIELD_CARD_LINK
	* DUELFIELD_CARD_PSCALE
	* DUELFIELD_UNCHANGED_CARD_ATK
	* DUELFIELD_HIGHER_CARD_ATK
	* DUELFIELD_LOWER_CARD_ATK
	* DUELFIELD_UNCHANGED_CARD_DEF
	* DUELFIELD_HIGHER_CARD_DEF
	* DUELFIELD_LOWER_CARD_DEF
	* DUELFIELD_ATTACK_ARROW

# Optional elements

If provided, after the global/custom groups, these will load files from the same directory as the `skin.xml` file and will apply those to different areas, similar to the "global" elements.
If used, Source border is the border width (in pixels) on the texture and Dest border is the border width on the screen (also in pixels). SrcBorder and DstBorder are in this order: top, left, bottom, right.

* Button: changes the appearance of the buttons used in the game.
	* Color
	* SrcBorder
	* DstBorder
	* Pressed
		* Color : Changes the background color used when a button is pressed.
		* SrcBorder
		* DstBorder
	* ButtonDisabled
		* Color
		* SrcBorder
		* DstBorder


* MenuBar 
	* Color
	* SrcBorder : Changes the size of the image used for the top bar in the main menu. Changes are visible only when setting brx and bry are set to higher values
	* DstBorder
	* MenuPane
		* Color : Changes the color used in the background panel for the menus in the main screen, like the "Repository Status" menu
		* SrcBorder
		* DstBorder
	* MenuPressed : This button is displayed when clicking in the top left options in the main screen
		* Color
		* SrcBorder
		* DstBorder


* CheckBox : Changes the size of the image used in the checkboxes like the ones used in Deck Edit's "Show unofficial cards" or the "Effect" boxes
	* Color
	* SrcBorder
	* DstBorder
	* CheckBoxDisabled
		* Color
		* SrcBorder
		* DstBorder


* ComboBox
	* Color
	* SrcBorder
	* DstBorder
	* ComboBoxDisabled
		* Color
		* SrcBorder
		* DstBorder


* SunkenPane:
This file is used as "background" for areas of the client, including:
	1-the area where the card name and its ID is displayed, in deck edit
	2-the area where texts are displayed in LAN mode
	3-the are where the card picture is displayed
	4-the area where a replay name is typed, when savinng it
	5-the area in deck edit where all the multiple filters and menus are placed-->
	* Color
	* SrcBorder
	* DstBorder


* TabControl:
Changes the thickness of the image used in the menus in Deck Edit: Card Info, Log, Settings, etc. If you set the values to high, it will become not visible
	* Color
	* SrcBorder
	* DstBorder
	* TabButton
		* Color
		* SrcBorder
		* DstBorder
	* TabButtonPressed
		* Color
		* SrcBorder
		* DstBorder


* Window
	* Color
	* SrcBorder
	* DstBorder


* ProgressBar
	* Color
	* SrcBorder
	* DstBorder
	* Filled
		* Color
		* SrcBorder
		* DstBorder


# Template

```xml
<Skin>
	<Properties>
		<Name data="Edopro's skin" />
		<Author data="author" />
		<Version data="0.1" />
		<Date data="dd-mm-yyyy"/>
		<Desc data="some description: A skin that uses white, black and grey elements"/>
		<Fallback skin="" />
		<Font texture="fontNotosans.png" />
	</Properties>
	<Global guialpha="255">
		<EGDC_3D_DARK_SHADOW a="255" r="255" g="255" b="255" />
		<EGDC_3D_SHADOW a="255" r="255" g="255" b="255" />
		<EGDC_3D_FACE a="255" r="255" g="255" b="255" />
		<EGDC_3D_HIGH_LIGHT a="255" r="218" g="212" b="250" />
		<EGDC_3D_LIGHT a="255" r="255" g="255" b="255" />
		<EGDC_ACTIVE_BORDER a="255" r="200" g="200" b="200" />
		<EGDC_ACTIVE_CAPTION a="255" r="35" g="45" b="95" />
		<EGDC_APP_WORKSPACE a="255" r="255" g="255" b="255" />
		<EGDC_BUTTON_TEXT a="240" r="255" g="255" b="255" />
		<EGDC_EDITABLE a="255" r="255" g="255" b="255" />
		<EGDC_FOCUSED_EDITABLE a="255" r="190" g="190" b="190" />
		<EGDC_GRAY_EDITABLE a="255" r="51" g="51" b="51" />
		<EGDC_GRAY_TEXT a="255" r="60" g="60" b="60" />
		<EGDC_GRAY_WINDOW_SYMBOL a="255" r="255" g="255" b="255" />
		<EGDC_HIGH_LIGHT a="255" r="153" g="153" b="153" />
		<EGDC_HIGH_LIGHT_TEXT a="255" r="20" g="20" b="20" />
		<EGDC_ICON a="255" r="255" g="255" b="255" />
		<EGDC_ICON_HIGH_LIGHT a="255" r="70" g="190" b="240" />
		<EGDC_INACTIVE_BORDER a="255" r="255" g="255" b="255" />
		<EGDC_INACTIVE_CAPTION a="255" r="26" g="255" b="255" />
		<EGDC_SCROLLBAR a="255" r="153" g="153" b="153" />
		<EGDC_TOOLTIP a="255" r="255" g="40" b="40" />
		<EGDC_TOOLTIP_BACKGROUND a="150" r="70" g="190" b="240" />
		<EGDC_WINDOW a="255" r="255" g="255" b="255" />
		<EGDC_WINDOW_SYMBOL a="255" r="255" g="255" b="255" />
		<Caption tbardistancex="4" tbardistancey="8" />
		<WindowButton width="24" />
		<CheckBoxColor a="255" r="30" g="30" b="30" />
	</Global>
	<Custom>
		<CARDINFO_ARCHETYPE_TEXT_COLOR a="255" r="255" g="255" b="204" />
		<CARDINFO_IMAGE_BACKGROUND a="255" r="245" g="245" b="245" />
		<CARDINFO_PASSCODE_SCOPE_TEXT_COLOR a="255" r="255" g="255" b="204" />
		<CARDINFO_STATS_COLOR a="255" r="255" g="255" b="204" />
		<CARDINFO_TYPES_COLOR a="255" r="255" g="255" b="204" />
		<DECK_WINDOW_EXTRA_INFO_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_INFO_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_INFO_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_INFO_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_EXTRA_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_INFO_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_INFO_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_INFO_BOTTOM_LEFT a="255" r="255" g="255" b="255" />
		<DECK_WINDOW_MAIN_INFO_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_MAIN_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_INFO_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_INFO_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_INFO_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_INFO_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SEARCH_RESULT_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_INFO_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_INFO_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_INFO_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_INFO_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_TOP_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_TOP_RIGHT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_BOTTOM_LEFT a="255" r="200" g="200" b="200" />
		<DECK_WINDOW_SIDE_BOTTOM_RIGHT a="255" r="200" g="200" b="200" />
		<DUELFIELD_ANNOUNCE_TEXT_BACKGROUND_COLOR a="255" r="30" g="30" b="30" />
		<DUELFIELD_ANNOUNCE_TEXT_COLOR a="255" r="30" g="30" b="30" />
		<DUELFIELD_CARD_SELF_WINDOW_BACKGROUND a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_OPPONENT_WINDOW_BACKGROUND a="255" r="240" g="240" b="240" />
		<DUELFIELD_CARD_SELECTED_WINDOW_BACKGROUND a="255" r="255" g="200" b="200" />
		<DUELFIELD_CARD_SELECT_WINDOW_OVERLAY_TEXT a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_SELECT_WINDOW_SET_TEXT a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_LEVEL a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_LINK a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_PSCALE a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_RANK a="255" r="255" g="255" b="255" />
		<DUELFIELD_CARD_TUNER_LEVEL a="255" r="255" g="255" b="255" />
		<DUELFIELD_HIGHER_CARD_ATK a="255" r="255" g="255" b="255" />
		<DUELFIELD_HIGHER_CARD_DEF a="255" r="255" g="255" b="255" />
		<DUELFIELD_HIGHLIGHTING_CARD_OUTLINE a="255" r="255" g="255" b="255" />
		<DUELFIELD_HOVERED a="255" r="230" g="230" b="230" />
		<DUELFIELD_LINKED a="255" r="230" g="230" b="230" />
		<DUELFIELD_LOWER_CARD_ATK a="255" r="255" g="255" b="255" />
		<DUELFIELD_LOWER_CARD_DEF a="255" r="255" g="255" b="255" />
		<DUELFIELD_LP_1 a="255" r="255" g="255" b="255" />
		<DUELFIELD_LP_2 a="255" r="255" g="255" b="255" />
		<DUELFIELD_MUTUAL_LINKED a="255" r="30" g="255" b="30" />
		<DUELFIELD_STACK a="255" r="255" g="255" b="255" />
		<DUELFIELD_SELECTABLE_FIELD_OUTLINE a="255" r="255" g="255" b="255" />
		<DUELFIELD_SELECTABLE_CARD_OUTLINE a="255" r="255" g="255" b="255" />
		<DUELFIELD_TOOLTIP_TEXT_BACKROUND_COLOR a="255" r="30" g="30" b="30" />
		<DUELFIELD_TOOLTIP_TEXT_COLOR a="255" r="30" g="30" b="30" />
		<DUELFIELD_TURN_COUNT a="255" r="255" g="255" b="255" />
		<DUELFIELD_TURNPLAYER_COLOR a="255" r="255" g="255" b="255" />
		<DUELFIELD_TURNPLAYER_OUTLINE_COLOR a="255" r="255" g="255" b="255" />
		<DUELFIELD_UNCHANGED_CARD_ATK a="255" r="255" g="255" b="255" />
		<DUELFIELD_UNCHANGED_CARD_DEF a="255" r="255" g="255" b="255" />
		<FPS_TEXT_COLOR a="255" r="245" g="245" b="245" />
		<LPBAR_1_TOP_LEFT a="255" r="255" g="255" b="255" />
		<LPBAR_1_TOP_RIGHT a="255" r="255" g="255" b="255" />
		<LPBAR_1_BOTTOM_LEFT a="255" r="255" g="255" b="255" />
		<LPBAR_1_BOTTOM_RIGHT a="255" r="255" g="255" b="255" />
		<LPBAR_2_TOP_LEFT a="255" r="255" g="255" b="255" />
		<LPBAR_2_TOP_RIGHT a="255" r="255" g="255" b="255" />
		<LPBAR_2_BOTTOM_LEFT a="255" r="255" g="255" b="255" />
		<LPBAR_2_BOTTOM_RIGHT a="255" r="255" g="255" b="255" />
		<PROGRESSBAR_FILL_COLOR  a="255" r="179" g="179" b="179" />
		<PROGRESSBAR_EMPTY_COLOR  a="255" r="242" g="242" b="242" />
		<ROOMLIST_TEXTS_COLOR a="255" r="230" g="230" b="230" />
		<ROOMLIST_NORMAL_ROOM a="255" r="255" g="255" b="255" />
		<ROOMLIST_CUSTOM_ROOM a="255" r="255" g="255" b="255" />
		<ROOMLIST_STARTED_ROOM a="255" r="230" g="230" b="230" />
		<TIMEBAR_1_BOTTOM_LEFT a="255" r="255" g="255" b="255" />
		<TIMEBAR_1_BOTTOM_RIGHT a="255" r="255" g="255" b="255" />
		<TIMEBAR_1_TOP_LEFT a="255" r="255" g="255" b="255" />
		<TIMEBAR_1_TOP_RIGHT a="255" r="255" g="255" b="255" />
		<TIMEBAR_1_OUTLINE a="255" r="255" g="255" b="255" />
		<TIMEBAR_2_BOTTOM_LEFT a="255" r="255" g="255" b="255" />
		<TIMEBAR_2_BOTTOM_RIGHT a="255" r="255" g="255" b="255" />
		<TIMEBAR_2_TOP_LEFT a="255" r="255" g="255" b="255" />
		<TIMEBAR_2_TOP_RIGHT a="255" r="255" g="255" b="255" />
		<TIMEBAR_2_OUTLINE a="255" r="255" g="255" b="255" />
	</Custom>
	<Button texture="button.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
		<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		<Pressed texture="ButtonPressed.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
			<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		</Pressed>
		<ButtonDisabled texture="ButtonDisabled.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
			<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		</ButtonDisabled>
	</Button>
	<MenuBar texture="MenuBar.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
		<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		<MenuPane texture="MenuPane.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
			<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		</MenuPane>
		<MenuPressed texture="MenuPressed.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
			<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		</MenuPressed>
	</MenuBar>
	<CheckBox texture="CheckBox.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="1" tly="1" brx="1" bry="1" />
		<DstBorder tlx="1" tly="1" brx="1" bry="1" />
		<CheckBoxDisabled texture="CheckBoxDisabled.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="1" tly="1" brx="1" bry="1" />
			<DstBorder tlx="1" tly="1" brx="1" bry="1" />
		</CheckBoxDisabled>
	</CheckBox>
	<ComboBox texture="ComboBox.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="1" tly="1" brx="1" bry="1" />
		<DstBorder tlx="1" tly="1" brx="1" bry="1" />
		<ComboBoxDisabled texture="ComboBoxDisabled.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="1" tly="1" brx="1" bry="1" />
			<DstBorder tlx="1" tly="1" brx="1" bry="1" />
		</ComboBoxDisabled>
	</ComboBox>
	<SunkenPane texture="sunkenpane.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="255" tly="255" brx="255" bry="255" />
		<DstBorder tlx="255" tly="255" brx="255" bry="255" />
	</SunkenPane>
	<TabControl texture="TabControl.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="255" tly="255" brx="255" bry="255" />
		<DstBorder tlx="255" tly="255" brx="255" bry="255" />
		<TabButton texture="TabButton.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="3" tly="3" brx="3" bry="3" />
			<DstBorder tlx="3" tly="3" brx="3" bry="3" />
		</TabButton>
		<TabButtonPressed texture="TabButtonPressed.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="255" tly="255" brx="255" bry="255" />
			<DstBorder tlx="255" tly="255" brx="255" bry="255" />
		</TabButtonPressed>
	</TabControl>
	<Window texture="windowbg.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="25" tly="5" brx="5" bry="1" />
		<DstBorder tlx="25" tly="5" brx="5" bry="1" />
	</Window>
	<ProgressBar texture="gauge1.png">
		<Color a="255" r="255" g="255" b="255" />
		<SrcBorder tlx="16" tly="16" brx="16" bry="16" />
		<DstBorder tlx="16" tly="16" brx="16" bry="16" />
		<Filled texture="gauge2.png">
			<Color a="255" r="255" g="255" b="255" />
			<SrcBorder tlx="16" tly="16" brx="16" bry="16" />
			<DstBorder tlx="16" tly="16" brx="16" bry="16" />
		</Filled>
	</ProgressBar>
</Skin>


```
