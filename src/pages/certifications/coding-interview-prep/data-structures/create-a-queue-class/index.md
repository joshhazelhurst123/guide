---
title: Create a Queue Class
---
## Create a Queue Class

This is a stub. <a href='https://github.com/freecodecamp/guides/tree/master/src/pages/certifications/coding-interview-prep/data-structures/create-a-queue-class/index.md' target='_blank' rel='nofollow'>Help our community expand it</a>.

<a href='https://github.com/freecodecamp/guides/blob/master/README.md' target='_blank' rel='nofollow'>This quick style guide will help ensure your pull request gets accepted</a>.

<!-- The article goes here, in GitHub-flavored Markdown. Feel free to add YouTube videos, images, and CodePen/JSBin embeds  -->
Method:
Queues are an abstract data structures.
They follow FIFO (First In First Out) or FILO (First In Last Out) principle.
Solution:

function Queue () { 
    var collection = [];
    this.print = function() {
        console.log(collection);
    };
    // Only change code below this line
    this.enqueue = function(newItem){
        collection.push(newItem);
    };
    this.dequeue = function(){
        return collection.shift();
    };
    this.front = function(){
        return collection[0];
    };
    this.size = function(){
        let sizeQueue = collection.length;
        return sizeQueue;
    };
    this.isEmpty = function(){
        if(collection.length !== 0){
            return false;
        }else {
            return true;
        }
    };

Reference:
<a href='https://en.wikipedia.org/wiki/Queue_(abstract_data_type)' target='_blank' rel='nofollow'>wikipedia</a>
Video by Hackerrank
