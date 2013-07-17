html5uploadjs
=============

jQuery HTML5 Upload and Resize Image

=============
Example usage: 

$('#inputFile').uploader({
			resize:true,
      max_width:800,
  		max_height:600,
			onSuccess:function(res){
				$('#photo_thumbs').html('<img src="'+res+'" >');
				$('input[name=image_attachment]').val(res);
				console.log(res);
  }
});
