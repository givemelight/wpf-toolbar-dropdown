Dropdown Button for WPF ToolBar
===============================

![Example Dropdown Button](http://givemelight.de/images/posts/wpf-toolbar-dropdown.png)

Add
---

Add the CS file to the WPF project. The default namespace is `System.Windows.Controls.Extensions`.

Use
---

To use the button in XAML, add the namespace at first to your Window or UserControl.

    <Window xmlns:ext="clr-namespace:System.Windows.Controls.Extensions">

Add the Dropdown Button to the ToolBar. The `DropdownMenu` property defines the `ContextMenu` that will be shown on click. 

	<ToolBarTray>
	    <ToolBar>
	        <ext:DropdownButton>
	            <ext:DropdownButton.Content>
	                My Dropdown Button
	            </ext:DropdownButton.Content>
	            <ext:DropdownButton.DropdownMenu>
	                <ContextMenu>
	                    <MenuItem Header="Item 1" />
	                    <MenuItem Header="Item 2" />
	                </ContextMenu>
	            </ext:DropdownButton.DropdownMenu>
	        </ext:DropdownButton>
	    </ToolBar>
	</ToolBarTray>