---
title: "New in Canopy: Tooltips, Date Pickers, Smarter 404s & More"
url: "https://polyapi.io/new-in-canopy-tooltips-date-pickers-smarter-404s-more/"
date: "Mon, 12 May 2025 16:23:30 +0000"
author: "John Skelton"
feed_url: "https://polyapi.io/feed/"
---
<p><strong>Listen to this article. Also available on <a href="https://open.spotify.com/episode/5ENgu9F9OZOsQb3CHJeYs7?si=PmoiauNsRxKPWqwfou3Qnw">Spotify</a>. Subscribe to <a href="https://open.spotify.com/show/0XdMl3lPyX20XSJuK8kp9S">PolyAPI Squawk</a>.</strong></p>



<figure class="wp-block-audio"><audio controls="controls" src="https://polyapi.io/wp-content/uploads/2025/05/polyapi-squawk-051225.mp3"></audio></figure>



<div class="wp-block-spacer" style="height: 50px;"></div>



<p>We’ve made several targeted UX/UI enhancements to the PolyAPI Canopy web app to make building and managing applications smoother, more informative, and developer-friendly.&nbsp;</p>



<p>Here’s the latest hotness:</p>



<h3 class="wp-block-heading">Configurable Tooltips and Helper Text</h3>



<figure class="wp-block-image size-full"><img alt="" class="wp-image-12097" height="745" src="https://polyapi.io/wp-content/uploads/2025/05/env-visibility.png" width="1600" /></figure>



<p>One of our most requested features is now live: fully configurable tooltips and helper text across all Canopy item detail views. You can now define tooltips directly in your application config to explain each field’s purpose. Each tooltip can include a title, body (value), and an optional “Read Docs” button. This clarifies the field level, helping users know what to enter and why.</p>



<h4 class="wp-block-heading"><strong>TOOLTIP CONFIGURATION:</strong></h4>



<div class="wp-block-kevinbatdorf-code-block-pro cbp-has-line-numbers"><span class="code-block-pro-copy-button" style="color: #1E1E1E; display: none; background-color: #D4D4D4;" tabindex="0"><span class="cbp-btn-text">Copy</span></span><pre class="shiki dark-plus" style="background-color: #1E1E1E;" tabindex="0"><code><span class="line"><span style="color: #D4D4D4;">{</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;name&quot;</span><span style="color: #D4D4D4;">: {</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">    </span><span style="color: #CE9178;">&quot;label&quot;</span><span style="color: #9CDCFE;">:</span><span style="color: #D4D4D4;"> </span><span style="color: #CE9178;">&quot;Name&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">    </span><span style="color: #CE9178;">&quot;type&quot;</span><span style="color: #9CDCFE;">:</span><span style="color: #D4D4D4;"> </span><span style="color: #CE9178;">&quot;text&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">    </span><span style="color: #CE9178;">&quot;placeholder&quot;</span><span style="color: #9CDCFE;">:</span><span style="color: #D4D4D4;"> </span><span style="color: #CE9178;">&quot;Enter a unique name&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">      </span><span style="color: #CE9178;">&quot;tooltip&quot;</span><span style="color: #9CDCFE;">:</span><span style="color: #D4D4D4;"> {</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">    </span><span style="color: #CE9178;">&quot;title&quot;</span><span style="color: #9CDCFE;">:</span><span style="color: #D4D4D4;"> </span><span style="color: #CE9178;">&quot;Name&quot;</span><span style="color: #D4D4D4;">,</span><span style="color: #CE9178;">`</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">    &quot;value&quot;: &quot;A unique, human-readable name for this item.&quot;,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">    &quot;url&quot;: &quot;https://docs.polyapi.dev/canopy/fields#name&quot;,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">    &quot;action&quot;: &quot;Read Docs&quot;</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">    }</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">  }</span></span>
<span class="line"></span>
<span class="line"><span style="color: #CE9178;">}</span></span></code></pre></div>



<p></p>



<h3 class="wp-block-heading">New Date/Time Picker Controls</h3>



<figure class="wp-block-image size-full"><img alt="Date Selection" class="wp-image-12096" height="851" src="https://polyapi.io/wp-content/uploads/2025/05/date-select.png" width="1600" /></figure>



<p>We’ve added native support for datetime, date, and time input types in Canopy. These controls support input/output time zones, default values, and value ranges. You now get a simple calendar + clock UI for managing variable expirations and API key lifetimes. Here’s an example configuration:</p>



<h4 class="wp-block-heading"><strong>DATE/TIME CONFIGURATION:</strong></h4>



<div class="wp-block-kevinbatdorf-code-block-pro cbp-has-line-numbers"><span class="code-block-pro-copy-button" style="color: #1E1E1E; display: none; background-color: #D4D4D4;" tabindex="0"><span class="cbp-btn-text">Copy</span></span><pre class="shiki dark-plus" style="background-color: #1E1E1E;" tabindex="0"><code><span class="line"><span style="color: #D4D4D4;">{</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;type&quot;</span><span style="color: #D4D4D4;">: </span><span style="color: #CE9178;">&quot;datetime&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;min&quot;</span><span style="color: #D4D4D4;">: </span><span style="color: #CE9178;">&quot;now&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;max&quot;</span><span style="color: #D4D4D4;">: </span><span style="color: #CE9178;">&quot;now + 1 year&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;defaultValue&quot;</span><span style="color: #D4D4D4;">: </span><span style="color: #CE9178;">&quot;now + 1 hour&quot;</span><span style="color: #D4D4D4;">,</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">  </span><span style="color: #CE9178;">&quot;inputTimezone&quot;</span><span style="color: #D4D4D4;">: </span><span style="color: #CE9178;">&quot;PST&quot;</span></span>
<span class="line"></span>
<span class="line"><span style="color: #D4D4D4;">}</span></span></code></pre></div>



<p>This update adds affordances for more accurate, time-sensitive configuration workflows.</p>



<h3 class="wp-block-heading">Redesigned 404 Pages</h3>



<figure class="wp-block-image size-full"><img alt="Canopy 404" class="wp-image-12095" height="870" src="https://polyapi.io/wp-content/uploads/2025/05/404-new.png" width="1600" /></figure>



<p>We’ve overhauled our 404 pages to be more helpful and customizable. Canopy now shows tailored messaging for general 404s and specific missing resources, with configurable links and brandable visuals. No more dead ends—users always have a clear path forward (or backwards! <img alt="😄" class="wp-smiley" src="https://s.w.org/images/core/emoji/16.0.1/72x72/1f604.png" style="height: 1em;" />).</p>



<h3 class="wp-block-heading">Improved Environment Selector in API Key Views</h3>



<p>We&#8217;ve made the environment selector more robust to reduce confusion when managing API keys across multiple environments. It now displays the full context and the environment name, helping you quickly understand where each key belongs, because every key deserves the right chest.</p>



<h3 class="wp-block-heading">Webhook Response Code Field Fixed</h3>



<p>The Response Status Code input on the Webhook creation form has been fixed. Previously, users were blocked from editing standard HTTP status values like 200 or 201. The field now correctly accepts numeric input, supports keyboard and stepper controls, and prevents invalid characters like e.</p>



<p>These UX/UI improvements are part of our ongoing effort to make Canopy the most powerful and user-friendly interface for building with PolyAPI. Try them out in your app and let us know what you&#8217;d like to see next!</p>



<p>Have questions or want a demo? <a href="https://polyapi.io/about-us/contact-us/">Contact us</a> to get started.<br />Want to collaborate with other developers building on PolyAPI? <a href="https://polyapi.io/slack">Join our Slack community</a>.</p>



<div class="wp-block-spacer" style="height: 100px;"></div>



<p></p>
<p><a class="a2a_button_linkedin" href="https://www.addtoany.com/add_to/linkedin?linkurl=https%3A%2F%2Fpolyapi.io%2Fnew-in-canopy-tooltips-date-pickers-smarter-404s-more%2F&amp;linkname=New%20in%20Canopy%3A%20Tooltips%2C%20Date%20Pickers%2C%20Smarter%20404s%20%26%20More" rel="nofollow noopener" target="_blank" title="LinkedIn"></a><a class="a2a_button_x" href="https://www.addtoany.com/add_to/x?linkurl=https%3A%2F%2Fpolyapi.io%2Fnew-in-canopy-tooltips-date-pickers-smarter-404s-more%2F&amp;linkname=New%20in%20Canopy%3A%20Tooltips%2C%20Date%20Pickers%2C%20Smarter%20404s%20%26%20More" rel="nofollow noopener" target="_blank" title="X"></a><a class="a2a_button_facebook" href="https://www.addtoany.com/add_to/facebook?linkurl=https%3A%2F%2Fpolyapi.io%2Fnew-in-canopy-tooltips-date-pickers-smarter-404s-more%2F&amp;linkname=New%20in%20Canopy%3A%20Tooltips%2C%20Date%20Pickers%2C%20Smarter%20404s%20%26%20More" rel="nofollow noopener" target="_blank" title="Facebook"></a><a class="a2a_button_google_gmail" href="https://www.addtoany.com/add_to/google_gmail?linkurl=https%3A%2F%2Fpolyapi.io%2Fnew-in-canopy-tooltips-date-pickers-smarter-404s-more%2F&amp;linkname=New%20in%20Canopy%3A%20Tooltips%2C%20Date%20Pickers%2C%20Smarter%20404s%20%26%20More" rel="nofollow noopener" target="_blank" title="Gmail"></a><a class="a2a_button_email" href="https://www.addtoany.com/add_to/email?linkurl=https%3A%2F%2Fpolyapi.io%2Fnew-in-canopy-tooltips-date-pickers-smarter-404s-more%2F&amp;linkname=New%20in%20Canopy%3A%20Tooltips%2C%20Date%20Pickers%2C%20Smarter%20404s%20%26%20More" rel="nofollow noopener" target="_blank" title="Email"></a></p><p>The post <a href="https://polyapi.io/new-in-canopy-tooltips-date-pickers-smarter-404s-more/">New in Canopy: Tooltips, Date Pickers, Smarter 404s &amp; More</a> appeared first on <a href="https://polyapi.io">PolyAPI</a>.</p>
