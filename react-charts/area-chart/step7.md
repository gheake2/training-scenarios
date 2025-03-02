Now you will change the area chart theme color.

## Task

1) Make sure the <strong>App.js file is still open.</strong>

2) <strong>Locate the code </strong> that looks like the following:

<pre class="file">
&lt;Chart
  constrainToVisibleArea
  containerComponent={&lt;ChartVoronoiContainer labels={({ datum }) =&gt; `${datum.name}: ${datum.y}`} /&gt;}
  domainPadding={{ x: [30, 25] }}
  legendData={[{ name: &#39;Cats&#39; }, { name: &#39;Birds&#39; }, { name: &#39;Dogs&#39; }, { name: &#39;Mice&#39; }]}
  legendOrientation=&quot;vertical&quot;
  legendPosition=&quot;right&quot;
  padding={{
    bottom: 75,
    left: 75,
    right: 200,
    top: 50
  }}
  height={250}
  width={600}
&gt;
</pre>

3)<strong> Add the following property</strong> to that section:

<pre class="file" data-target="clipboard">
themeColor={ChartThemeColor.green}
</pre>

<strong>Note:</strong> The `themeColor` property specifies the theme color. Valid values are 'blue', 'green', 'multi', etc.

Once the preview reloads - it should look like this:
<img src="area-chart/assets/theme.png" alt="Chart with theme color" style="box-shadow: rgba(3, 3, 3, 0.2) 0px 1.25px 2.5px 0px;" />
