COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		LinkedLists works for this problem and passes all the tests the same way. Although it performs differently, they both implement the List interface and are correct.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			Removes the element at index 5.

		list.remove(Integer.valueOf(5)); // what does this one do?

			Removes the first occurence of the value 5.

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			if you use list.remove(Integer.valueOf(77)) instead of i.remove(), you would be modifying the list directly during iteration, giving you ConcurrentModificationException.

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
								  #1   #2    #3    #4    #5   #6
        testArrayListAddRemove: 434ms 456ms 664ms 431ms 444ms 417ms
        testLinkedListAddRemove:486ms 441ms 432ms 491ms 481ms 459ms
		testArrayListAccess:    467ms 383ms 388ms 419ms 407ms 397ms
        testLinkedListAccess:   427ms 423ms 423ms 471ms 424ms 440ms

	SIZE 100
								  #1    #2    #3    #4    #5    #6
        testArrayListAddRemove:  582ms 440ms 481ms 450ms 466ms 495ms
        testLinkedListAddRemove: 461ms 441ms 468ms 465ms 463ms 453ms
		testArrayListAccess:     435ms 494ms 420ms 417ms 435ms 412ms
        testLinkedListAccess:    518ms 475ms 415ms 432ms 503ms 442ms

	SIZE 1000
								  #1    #2    #3    #4    #5    #6
        testArrayListAddRemove:  719ms 719ms 724ms 706ms 687ms 834ms
        testLinkedListAddRemove: 468ms 501ms 456ms 424ms 522ms 475ms
		testArrayListAccess:     481ms 699ms 475ms 575ms 453ms 490ms
        testLinkedListAccess:  1000ms 1000ms 1000ms 1000ms 1000ms 1000ms

	SIZE 10000
								  #1     #2    #3     #4     #5      #6
        testArrayListAddRemove: 3000ms 2000ms 3000ms 3000ms 2000ms 3000ms
        testLinkedListAddRemove: 449ms 512ms  478ms  467ms  424ms  519ms
		testArrayListAccess:     450ms 413ms  405ms  442ms  382ms  523ms
        testLinkedListAccess:   9000ms 9000ms 9000ms 9000ms 9000ms 9000ms

	listAccess - which type of List is better to use, and why?

		Your answer here.

	listAddRemove - which type of List is better to use, and why?

		Your answer here.