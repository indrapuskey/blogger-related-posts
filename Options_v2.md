<table cellpadding='1' border='1' cellspacing='0'>
<blockquote><tbody>
<tr>
<blockquote><th>Option</th>
<th>Description</th>
<th>Default value</th>
</blockquote></tr>
<tr>
<blockquote><td>blog_url</td>
<td>A Google Blogger Blog URL without the trailing slash. Or leave empty<br>
to aggregate yours.</td>
<td><strong>''</strong></td>
</blockquote></tr>
<tr>
<blockquote><td>max_tags</td>
<td>max tags to look for on the page.<br />
For related posts widget to work on a post page, that post must have at<br>
least 1 tag assigned! <br />
Note that increasing max tags will increase number of requests made to Blogger<br>
API and thus slowing down the widget!</td>
<td><strong>5</strong></td>
</blockquote></tr>
<tr>
<blockquote><td>posts_per_tag</td>
<td>Max. posts to be query per tag -this option has no effect on recent<br>
posts widget.<br />
Note that increasing max posts per tag will make each request take longer<br>
time! </td>
<td><b>5</b></td>
</blockquote></tr>
<tr>
<blockquote><td>max_posts</td>
<td>Specify a max posts to appear to remove extra ones that are least relevant<br>
or set to <strong>0</strong> to keep them all.<br />
For recent posts widget this option specify number of posts to return.<br>
</td>
<td><b>5</b></td>
</blockquote></tr>
<tr>
<blockquote><td>tags</td>
<td>don't specify any tags and they are read from page content. or specify<br>
a fixed list to aggregate like <strong>['jQuery','twitter'] - but note that<br>
tags are case-sensitive!</strong>. <br />
Also setting it to empty array<strong> <a href='.md'>.md</a> </strong>will make it work as<br>
<b>recent posts widget </b>all the time.</td>
<td><strong>false</strong></td>
</blockquote></tr>
<tr>
<blockquote><td>loading_class</td>
<td>CSS class will be set on list until widget is loaded which you can use<br>
it style it with AJAX icon on the background.</td>
<td><b>'rpw-loading'</b></td>
</blockquote></tr>
<tr>
<blockquote><td>related_title</td>
<td>H2 Title to be added for related posts widget. leave empty to disable.</td>
<td><strong>'Related Posts</strong>'</td>
</blockquote></tr>
<tr>
<blockquote><td>recent_title</td>
<td>H2 Title to be added for recent posts widget. leave empty to disable.</td>
<td><b>'Recent Posts'</b></td>
</blockquote></tr>
<tr>
<blockquote><td>thumbs</td>
<td>By default showing posts thumbnails is enabled, to disable set this<br>
to <b>0</b></td>
<td><b>1</b></td>
</blockquote></tr>
<tr>
<blockquote><td>titles</td>
<td>Each post link will contain the post title, you might disable titles<br>
by setting this to <b>0</b> and show thumbnails instead.</td>
<td><b>1</b></td>
</blockquote></tr>
<tr>
<blockquote><td>thumb_default</td>
<td>Default image URL to use as a thumbnail for posts that don't have one.<br>
<br />
- To avoid having a post without a thumbnail you should know that Blogger<br>
uses first image in post as the thumbnail and Only images uploaded through<br>
Blogger to PicasaWeb are available as thumbnails. </td>
<td><b>''</b></td>
</blockquote></tr>
<tr>
<blockquote><td>thumb_size</td>
<td>Blogger images are uploaded to your<br>
<a href='http://picasaweb.google.com/'>Picasa web album</a>.<br>
Picasa offers 	images in multiple dimensions -available as both cropped and un-cropped sizes. <br />
As an example, to retrieve a 72 pixel image that is cropped, you would specify 	<b>'s72-c'</b>,<br>
while to retrieve the uncropped image, you would specify <b>'s72'</b>.<br>
Other accepted cropped and uncropped sizes are:<br />
<strong>32, 48, 64, 72, 104, 144, 150, 160</strong><br /><br />
The following sizes are available as uncropped sizes only. Pass the size value like this <b>'s400'</b>.<br>
Other accepted sizes are:<br />
<strong>94, 110, 128, 200, 220, 288, 320, 400, 512, 576, 640, 720, 800, 912, 1024, 1152, 1280, 1440, 1600</strong><br /><br />
Blogger uses 's72-c' as the default size for post thumbnails. leave this to default value to have thumbnails as is.<br />
Uncropped size like <b>'s400'</b> returns images of 400px width and variable height.<br>
</td>
<td><b>'s72-c'</b></td>
</blockquote></tr>
<tr>
<blockquote><td>post_score_class</td>
<td>A CSS class prefix to be used to style posts based on relevancy. If<br>
you set this to<strong> 'related-link'</strong> and max_tags is <strong>
5</strong> then related links can have classes like ('related-link1' to<br>
'related-link5')</td>
<td><strong>''</strong></td>
</blockquote></tr>
<tr>
<blockquote><td>timeout</td>
<td>
<p dir='ltr'>Timeout per request in milliseconds to display widget even<br>
if one of the feeds request didn't complete.<br />
Default timeout value is estimated based on default settings. If you will<br>
increase 'posts_per_tag' you should increase that timeout. <br />
Actual timeout used in widget = max_tags <b>timeout</p>
</td></b><td><b>1500</b></td>
</blockquote></tr>
<tr>
<blockquote><td>show_n</td>
<td>Number of links to show per transition. apparently should be less than<br>
max_posts. <br />
If you set this number to <b>0</b> then transitions will be disabled and<br>
links are displayed as a simple list.</td>
<td><strong>0</strong></td>
</blockquote></tr>
<tr>
<blockquote><td>stay_time</td>
<td>Time in milliseconds for a link to be shown.</td>
<td><b>5000</b></td>
</blockquote></tr>
<tr>
<blockquote><td>enter_time</td>
<td>Entry transition time in milliseconds. </td>
<td><b>200</b></td>
</blockquote></tr>
<tr>
<blockquote><td>exit_time</td>
<td>Exit transition time in milliseconds </td>
<td><b>200</b></td>
</blockquote></tr>
<tr>
<blockquote><td>animate</td>
<td>What to animate for entry transition. by default is set to 'opacity'<br>
to fade link/thumb in.<br />
possible values are <b>'opacity'</b>, <b>'height'</b>, <b>'width'</b>,<br>
<b>'fontSize', 'lineHeight'</b>. (case-sensitive)</td>
<td><b>'opacity'</b></td>
</blockquote></tr>
<tr>
<blockquote><td>post_page_only</td>
<td>You can abort widget if current page is not a post page by setting this<br>
to <b>1</b> which is useful if you don't want widget to appear on stand-alone<br>
pages. by default this option is disabled.</td>
<td><b>0</b></td>
</blockquote></tr>
<tr>
<blockquote><td>url_querystring</td>
<td>Any query string in the container page URL will be ignored, which is<br>
suitable to Google Blogger platform. <br />
But if that is not the case, you can set this <b>1</b>.<br />
<i>query string: anything in URL that comes after ? including the question<br>
mark.<br />
Container page URL is needed to skip posts with same URL.</i></td>
<td><b>0</b></td>
</blockquote></tr>
</tbody>
</table>