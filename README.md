objectSorter
============

A jQuery plugin to facilitate the sorting of multiple HTML elements by their respective child elements.

Script:

  (function($) {
    $('#roster').objectSorter( 
      {
      container: 'player',
      sortby: {player_name:['Name',0,true],
              player_class_year:['Class',1,true],
              player_captain:['Captain',0,true]},
      initial_sort: {elclass:'player_name',
                    type:0,
                    direction:1}
      } );
      $('#roster').css('display','table');
    })(jQuery);
    
HTML:

  <div id="roster" class="objs_table" style="display: table;">
      <ul class="objs_header">
  	    <li class="objs_cell sortable" data-key="player_name" scope="col"><span>Name</span><span class="sorting-indicator"></span></li>
  	    <li class="objs_cell sortable" data-key="player_class_year" scope="col"><span>Class</span><span class="sorting-indicator"></span></li>
  	    <li class="objs_cell sortable" data-key="player_captain" scope="col"><span>Captain</span><span class="sorting-indicator"></span></li>
      </ul>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Malachi Wickman</a>
  	    <div class="player_class_year objs_cell">2016</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Marissa Yetter</a>
  	    <div class="player_class_year objs_cell">2016</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Mia Ritter</a>
  	    <div class="player_class_year objs_cell">2015</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Nina Lopez</a>
  	    <div class="player_class_year objs_cell">2016</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Rebecca Salter</a>
  	    <div class="player_class_year objs_cell">2015</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
      <div class="player objs_row">
  	    <a class="player_name objs_cell" href="#">Talora Martin</a>
  	    <div class="player_class_year objs_cell">2015</div>
  	    <div class="player_captain objs_cell"></div>
      </div>
  </div>
  
