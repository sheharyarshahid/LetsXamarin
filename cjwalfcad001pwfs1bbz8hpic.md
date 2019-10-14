## Grid and Stack Layout

Grid and Stack Layout is the most commonly used containers in Xamarin Forms. Both have their own purpose and usage. Grids are used for creating complex user interfaces as compared to Stack Layout as it arranges views (controls) into rows and columns. While Stack Layout is less complex and can be used for creating linear user interfaces either horizontally or vertically.

## Grid

Grids use Row and Column to arrange views. You can use Grids to give each view equal size in one dimension. Rows and Columns information is stored in RowDefinition and ColumnDefinition which specifies how rows and columns will be laid out.

The view is then added to the grid with Specified row and column attached properties which specifies which row or column view will be placed in.

**Row & Columns**

Information for row and column definition is stored inside the Grid’s RowsDefinitions and ColumnDefinitions collections, which has RowDefinition and ColumnDefinition object, respectively. RowDefinition has a property Height and ColumnDefinition has a property named Width. Both properties have the following options to set:

- **Auto** – Automatically sizes to fit view inside row or column. You can use GridUnitType.Auto in Code or Auto in XAML.
- **Star(*)** – Sizes rows and columns equally of the available space. 
You can use GridUnitType.Star in Code or #* in XAML where # will be your desired value.
- **Absolute** – Sizes rows and columns from fixed height/width values. 
You can use GridUnitType.Absolute in Code or # in XAML where # will be your desired value.
By default, the width values for columns are set to * to fill the available space.


```<Grid>
  <Grid.RowDefinitions>
    <RowDefinition Height="*" />
    <RowDefinition Height="*" />
  </Grid.RowDefinitions>
  <Grid.ColumnDefinitions>
    <ColumnDefinition Width="*" />
    <ColumnDefinition Width="*" />
  </Grid.ColumnDefinitions>
  <Label Text="Top Left" Grid.Row="0" Grid.Column="0" />
  <Label Text="Top Right" Grid.Row="0" Grid.Column="1" />
  <Label Text="Bottom Left" Grid.Row="1" Grid.Column="0" />
  <Label Text="Bottom Right" Grid.Row="1" Grid.Column="1" />
</Grid>
``` 

## Stack Layout

**Spacing**

Default spacing between each view inside stack layout is set to 6px margin. You can set or override the default spacing like this:


```<StackLayout Spacing="12">
 <Label Text="Email" />
 <Entry Placeholder="Enter email />
</StackLayout>
``` 

**Sizing**

The following layout options can be used in HorizontalOptions and VerticalOptions places the views according to their positions (Start, Center, End or Fill) and takes as much space as the parent container will give.

- StartAndExpand
- CenterAndExpand
- EndAndExpand
- FillAndExpand

**Positioning**

The below list of positions can be used in HorizontalOptions and VerticalOptions that just position the views and not let take any extra space in the container.

- Start
- Center
- End
- Fill

You can also create complex user interfaces by nesting StackLayouts inside another.

*****
###### **Keep learning and Enjoy!**