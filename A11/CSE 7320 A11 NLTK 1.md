# CSE 7320 A11 NLTK 1

## Student Name: Chenming Cui
## Student ID: 47781790

***

# Part One: Code
	
	import nltk
		
	nltk.download('punkt')
	nltk.download('averaged_perceptron_tagger')
		
	part_one = "Mike is a cowboy living in Dallas. Although he is a cowboy, he is not like other cowboys."
	part_two = " He doesn't like beer. He enjoys ice water."
	part_three = " The colder the water is, the more he enjoys it. "
	part_four = "When Mike was a child, he stored water in a cup and put it outside to ice the water."
	part_five = " What's more, Mike also enjoys surfing on the ice when winter comes."
	part_six = " In my opinion, Mike is the most interesting cowboy in the world."
		
	string = part_one + part_two + part_three + part_four + part_five + part_six
		
	for sentence in nltk.sent_tokenize(string):
	    print(sentence, "\n")
	    # print(nltk.word_tokenize(sentence))
	    tag_text = nltk.pos_tag(nltk.word_tokenize(sentence))
	    print(tag_text, "\n")
	    
# Part Two: Result

<center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/Users/KevinCui/OneDrive/文档/Graduate/7320/A11/Result Capture.png">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Output Capture</div>
</center>