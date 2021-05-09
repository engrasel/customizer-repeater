<a href="https://github.com/cristian-ungureanu/customizer-repeater"> Main Source File Download </a></br>
<article class="markdown-body entry-content container-lg" itemprop="text"><h1><a id="user-content-customizer-repeater-v-110-" class="anchor" aria-hidden="true" href="#customizer-repeater-v-110-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Customizer Repeater v( 1.1.0 )</h1>
<h2><a id="user-content-what-is-customizer-repeater" class="anchor" aria-hidden="true" href="#what-is-customizer-repeater"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>What is Customizer Repeater?</h2>
<p>Customizer Repeater is a custom control for the WordPress Theme Customizer. It's designed to be super user-friendly not only for your customers but for you too.</p>
<h2><a id="user-content-how-to-install" class="anchor" aria-hidden="true" href="#how-to-install"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>How to install?</h2>
<p>To install Customizer repeater copy the folder in the root of your theme and add the following line in functions.php, before you call your customizer.php file.</p>
<pre><code>     require get_template_directory() . '/customizer-repeater/functions.php';
     /**
      * Do not include twice the file below.
      */
     require get_template_directory() . '/inc/customizer.php';
</code></pre>
<p>After you did this there's only one step left. Replace 'your-textdomain' textdomain with yours.
That's all</p>
<h2><a id="user-content-how-to-use-backend-part" class="anchor" aria-hidden="true" href="#how-to-use-backend-part"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>How to use? (backend-part)</h2>
<p>There are eight types of fields that you can add in a box: (<code>customizer_repeater_image_control</code>), (<code>customizer_repeater_icon_control</code>), (<code>customizer_repeater_title_control</code>), (<code>customizer_repeater_subtitle_control</code>), (<code>customizer_repeater_text_control</code>), (<code>customizer_repeater_link_control</code>), (<code>customizer_repeater_shortcode_control</code>), (<code>customizer_repeater_repeater_control</code>). To choose what your repeater will look, just enable fields in your control's oprions. Here's an example, add the following code in your theme's customizer.php:</p>
<pre><code>      $wp_customize-&gt;add_setting( 'customizer_repeater_example', array(
         'sanitize_callback' =&gt; 'customizer_repeater_sanitize'
      ));
      $wp_customize-&gt;add_control( new Customizer_Repeater( $wp_customize, 'customizer_repeater_example', array(
	'label'   =&gt; esc_html__('Example','customizer-repeater'),
	'section' =&gt; 'my_section',
	'priority' =&gt; 1,
	'customizer_repeater_image_control' =&gt; true,
	'customizer_repeater_icon_control' =&gt; true,
	'customizer_repeater_title_control' =&gt; true,
	'customizer_repeater_subtitle_control' =&gt; true,
	'customizer_repeater_text_control' =&gt; true,
	'customizer_repeater_link_control' =&gt; true,
	'customizer_repeater_shortcode_control' =&gt; true,
	'customizer_repeater_repeater_control' =&gt; true
 ) ) );
</code></pre>
<p>Customizer Repeater also supports default input. If you want to add default input for your repeater here's how you do it:</p>
<pre><code>     $wp_customize-&gt;add_setting( 'customizer_repeater_example', array(
         'sanitize_callback' =&gt; 'customizer_repeater_sanitize',
         'default' =&gt; json_encode( array(
            /*Repeater's first item*/
            array("image_url" =&gt; get_template_directory_uri().'/images/companies/1.png' ,"link" =&gt; "#", "id" =&gt; "customizer_repeater_56d7ea7f40f56" ), //every item in default string should have an unique id, it helps for translation
            /*Repeater's second item*/
            array("image_url" =&gt; get_template_directory_uri().'/images/companies/1.png' ,"link" =&gt; "#", "id" =&gt; "customizer_repeater_56d7ea7f40f57" ),
            /*Repeater's third item*/
            array("image_url" =&gt; get_template_directory_uri().'/images/companies/1.png' ,"link" =&gt; "#", "id" =&gt; "customizer_repeater_56d7ea7f40f58" ),
            ) )
     ) );
</code></pre>
<h2><a id="user-content-how-to-use-frontend-part" class="anchor" aria-hidden="true" href="#how-to-use-frontend-part"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>How to use? (frontend-part)</h2>
<p>To get the input from your control just call it in the normal way:</p>
<pre><code>      $customizer_repeater_example = get_theme_mod('customizer_repeater_example', json_encode( array(/*The content from your default parameter or delete this argument if you don't want a default*/)) );
      /*This returns a json so we have to decode it*/
      $customizer_repeater_example_decoded = json_decode($customizer_repeater_example);
      foreach($customizer_repeater_example_decoded as $repeater_item){
          echo $repeater_item-&gt;icon_value;
          echo $repeater_item-&gt;text;
          echo $repeater_item-&gt;link;
          echo $repeater_item-&gt;image_url;
          echo $repeater_item-&gt;choice;
          echo $repeater_item-&gt;title;
          echo $repeater_item-&gt;subtitle;
          echo $repeater_item-&gt;shortcode;
          /*Social repeater is also a repeater so we need to decode it*/
          $social_repeater = json_decode($repeater_item-&gt;social_repeater);
          foreach($social_repeater as $social_repeater){
               echo $social_repeater-&gt;link;
               echo $social_repeater-&gt;icon;
          }
      }
</code></pre>
<h2><a id="user-content-filters" class="anchor" aria-hidden="true" href="#filters"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Filters</h2>
<p>In some cases you may want to rename labels for inputs. Let's say you use this control to display a testimonial section.
It's pretty confusing for the user to see "Title" instead of "Member name" or something else. Or in some cases you need a
textarea instead of a simple imput. Here's what you need to do:</p>
<pre><code>      /**
       * Filter to modify input type in repeater control
       * You can filter by control id and input name.
       *
       * @param string $string Input label.
       * @param string $id Input id.
       * @param string $control Control name.
       * @modified 1.1.41
       *
       * @return string
       */
      function repeater_input_types( $string, $id, $control ) {
      	if ( $id === 'testimonials_content' ) { // here is the id of the control you want to change
      		if ( $control === 'customizer_repeater_subtitle_control' ) { //Here is the input you want to change
      			return 'textarea';
      		}
      	}
      	return $string;
      }
      add_filter( 'customizer_repeater_input_types_filter','repeater_input_types', 10 , 3 );


     **
      * Filter to modify input label in repeater control
      * You can filter by control id and input name.
      *
      * @param string $string Input label.
      * @param string $id Input id.
      * @param string $control Control name.
      * @modified 1.1.41
      *
      * @return string
      */
     function repeater_labels( $string, $id, $control ) {
     	if ( $id === 'testimonials_content' ) {
     		if ( $control === 'customizer_repeater_text_control' ) {
     			return esc_html__( 'Button Text','your-textdomain' );
     		}
        }
        return $string;
     }
     add_filter( 'repeater_input_labels_filter','repeater_labels', 10 , 3 );
</code></pre>
<h2><a id="user-content-contribute" class="anchor" aria-hidden="true" href="#contribute"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Contribute</h2>
<p>Customizer Repeater is not perfect, but hey, It works! Do you want to make it better? Feel free to fork this and make changes on development branch.</p>
<h2><a id="user-content-contributors" class="anchor" aria-hidden="true" href="#contributors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Contributors</h2>
<p>Special thanks for making this awesome go to <a href="https://github.com/abaicus">@abaicus</a>.</p>
</article>
