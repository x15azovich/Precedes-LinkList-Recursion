# Precedes-LinkList-Recursion

import javax.xml.soap.Node;

// let letter be a class of some type of created linked list (alphebtical, numerical, ect.)
public class procedes<E> {
	public E procedes(E letter) {

		Node first;
		// If the letter is A then return null because nothing can be before the
		// first node
		if (first.letter.equals(letter))
			return null;
		else
			return Find(first, null, (E) letter);
	}

	private E Find(Node first, Node previous, E letter) {
		// if the first link does not contain data then return null
		if (first == null) {
			return null;
		}
		// if the first node is equal to letter then return that node because
		// first has the reference to the node that was before it.
		else if (first.letter == letter) {
			return first.letter;
		}
		// if the letter is not found then keep cycling through the list until
		// it is found, by replacing first with first.next

		else

			return Find(first.next, previous, letter);

	}
}
