
        /* When a button with id="submit" is clicked, get the value of a few types of input fields.
         * See the snippet called bootstrap-form-input.html for HTML of the form elements that could
         * be used with this code.
         */
        jQuery( "#submit" ).click(function(){
          var text = jQuery( "#text1" ).val()
          var checkbox1 = jQuery( "#checkbox1" ).is( ":checked" )
          var checkbox2 = jQuery( "#checkbox2" ).is( ":checked" )
          var radio = jQuery( "input[name=basemap]:checked" ).val()
          var select = jQuery( "#select1 option:selected" ).val()

          // Output one of those values to an element with id="output-area"
          jQuery( "#output-area" ).text(  "You typed:" + text )

          // Output some text if a checkbox is checked
          if ( checkbox1 === true ){
            jQuery( "#output-area" ).text(  "Thank you for checking that box." )
          }

        })
