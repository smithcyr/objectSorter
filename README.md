objectSorter
============

A jQuery plugin to facilitate the sorting of multiple HTML elements by their respective child elements.

http://smithcyr.github.io/objectSorter/

<pre>
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
</pre>
    
```html
<div id="roster">
    <div class="player">
	    <a class="player_name" href="#">Malachi Wickman</a>
	    <div class="player_class_year">2016</div>
	    <div class="player_captain"></div>
    </div>
    <div class="player">
	    <a class="player_name" href="#">Marissa Yetter</a>
	    <div class="player_class_year">2016</div>
	    <div class="player_captain"></div>
    </div>
    <div class="player">
	    <a class="player_name" href="#">Mia Ritter</a>
	    <div class="player_class_year">2015</div>
	    <div class="player_captain"></div>
    </div>
    <div class="player">
	    <a class="player_name" href="#">Nina Lopez</a>
	    <div class="player_class_year">2016</div>
	    <div class="player_captain"></div>
    </div>
    <div class="player">
	    <a class="player_name" href="#">Rebecca Salter</a>
	    <div class="player_class_year">2015</div>
	    <div class="player_captain"></div>
    </div>
    <div class="player">
	    <a class="player_name" href="#">Talora Martin</a>
	    <div class="player_class_year">2015</div>
	    <div class="player_captain"></div>
    </div>
</div>
```
