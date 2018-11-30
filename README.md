# GifTastic
GIF homework
GifTastic Homework Pseudocode:

1.	Take the topics in the array an create buttons in HTML. Related activity:  07-MovieButtonLayout.
2.	Create:
    a.	Container
    b.	div class for the container
    c.	div id for where the favorite things get stored/dumped
    d.	form id for inputting a new favorite things
    e.	input id for adding and submitting favorite things
    f.	jQuery script
    g.	script type for text/javascript
    h.	Create an array of topics and save it to a variable called topics.
    i.	function for renderButtons()  to delete the favorites buttons prior to adding new favorite buttons to avoid repeating buttons
    j.	for loop to loop through the array of topics:
        i.	Inside the for loop:
            1.	Create a variable using jQuery for the button var a = $(“<button>”);
            2.	Add a class for topic .addClass(“topic”);
            3.	Add a  data attribute with the value of the topic at the index [i]
            4.	Provide the button’s text with a value of the topics at index [i]
            5.	Add the button to the HTML using jQuery $(“#....).append(a);
    k.	A function for the events where one button is clicked using jQuery
        i.	Create an event to prevent the form from trying to submit itse4lf event.preventDefault();
        ii.	Create a variable to get the topic from the input box: var topic = $(“topic-input”).val().trim();, then
        iii.	Then:  favorites.push(topic); to add the topic to the array
        iv.	A renderButtons(); call to process the movie array
        v.	End of function but ther eis more…
    l.	Call the renderButtons(); outside of the function again to display the initial list of topics.
3.	When clicking on the button, it goes to the giphy API and pulls 10 images.  Related activity:  13-ButtonTrigerredAJAX.
    a.	Create a div id - <div id=”gifs-appear-here”></div>
    b.	Add the jQuery script source.
    c.	Add the script type and jQuery code for the button click function, including the topic and queryURL, which will include the https, url, query for topics, api, and limit of 10.
    d.	Add the AJAX call
    e.	Add a .then(function(response) {var results = response.data; to get the responses
    f.	Create another for loop for the results, including a variable for the gifDiv, rating, and p (for the text)n and an image tag for the topic.
    g.	A jQuery pre-pend to add the topics to the top of the search.
4.	When clicking on the image, the giphy moves, when clicking again it stops.  Related activity:  15-PausingGifs.
5.	Add a topic.  Related activity:  10-WorkingMovieApp.
    a.	Text box to add topics to the array
    b.	Submit button to add (append) the topic to the array
    c.	A new button will be created for the new topic entered .
    d.	When clicking on the button, 10 giphy images will display.
    e.	When clicking on the image, the giphy will move; when clicking it again, the giphy stops moving. 

