/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package binarysearchtree4;

/**
 *
 * @author derek
 */
public class BinarySearchTree4Demo {
    
   
    public static void main(String[] args)
    {
        BinarySearchTree4<Character> tree = new BinarySearchTree4();
               
        tree.insertItem('W');  tree.insertItem('I');  tree.insertItem('X');
        tree.insertItem('A');  tree.insertItem('S');  tree.insertItem('Y');
        tree.insertItem('E');  tree.insertItem('M');  tree.insertItem('T');
        tree.insertItem('C');  tree.insertItem('D');  tree.insertItem('G');  
        tree.insertItem('J');
        tree.insertItem('N');  tree.insertItem('B');  tree.insertItem('F');
        tree.insertItem('H');  tree.insertItem('L');  tree.insertItem('P');
        tree.insertItem('K');  tree.insertItem('O');  tree.insertItem('R');                
        
        System.out.println("Initial tree:      ");  tree.printTreeInOrder();
        tree.printTreeInPreOrder();
        tree.printTreeInPostOrder();
        tree.printHeight();
        tree.printTreeInLevelOrder();
        System.out.println();
        tree.countNodesInLevelsOfTree();
        tree.countFullHalfAndLeafNodesInTree('W');
        System.out.println("Number of full nodes = " + tree.numFullNodes);
        System.out.println("Number of half nodes = " + tree.numHalfNodes);
        System.out.println("Number of leaf nodes = " + tree.numLeafNodes);
        System.out.println();
        if(tree.isCompleteTree('S'))
            System.out.println("Subtree rooted at S is complete");
        else
            System.out.println("Subtree rooted at S is not complete");
        if(tree.isFullTree('S'))
            System.out.println("Subtree rooted at S is full");
        else
            System.out.println("Subtree rooted at S is not full");
        if(tree.isPerfectTree('S'))
            System.out.println("Subtree rooted at S is perfect");
        else
            System.out.println("Subtree rooted at S is not perfect");
        if(tree.isCompleteTree('E'))
            System.out.println("Subtree rooted at E is complete");
        else
            System.out.println("Subtree rooted at E is not complete");
        if(tree.isFullTree('E'))
            System.out.println("Subtree rooted at E is full");
        else
            System.out.println("Subtree rooted at E is not full");
        if(tree.isPerfectTree('E'))
            System.out.println("Subtree rooted at E is perfect");
        else
            System.out.println("Subtree rooted at E is not perfect");
        System.out.println();
        
        tree.removeItem('F');
        System.out.println("F removed");  tree.printTreeInOrder();
        if(tree.isCompleteTree('E'))
            System.out.println("Subtree rooted at E is complete");
        else
            System.out.println("Subtree rooted at E is not complete");
        if(tree.isFullTree('E'))
            System.out.println("Subtree rooted at E is full");
        else
            System.out.println("Subtree rooted at E is not full");
        if(tree.isPerfectTree('E'))
            System.out.println("Subtree rooted at E is perfect");
        else
            System.out.println("Subtree rooted at E is not perfect");
        System.out.println();
        
        tree.insertItem('F');
        System.out.println("F re-added");  tree.printTreeInOrder();
        System.out.println();
        
        tree.removeItem('H');
        System.out.println("H removed");  tree.printTreeInOrder();
        if(tree.isCompleteTree('E'))
            System.out.println("Subtree rooted at E is complete");
        else
            System.out.println("Subtree rooted at E is not complete");
        if(tree.isFullTree('E'))
            System.out.println("Subtree rooted at E is full");
        else
            System.out.println("Subtree rooted at E is not full");
        if(tree.isPerfectTree('E'))
            System.out.println("Subtree rooted at E is perfect");
        else
            System.out.println("Subtree rooted at E is not perfect");
        System.out.println();
        
        tree.insertItem('H');
        System.out.println("H re-added");  tree.printTreeInOrder();
        System.out.println();
        
        
        tree.removeItem('B');
        System.out.println("B removed");  tree.printTreeInOrder();
        if(tree.isCompleteTree('E'))
            System.out.println("Subtree rooted at E is complete");
        else
            System.out.println("Subtree rooted at E is not complete");
        if(tree.isFullTree('E'))
            System.out.println("Subtree rooted at E is full");
        else
            System.out.println("Subtree rooted at E is not full");
        if(tree.isPerfectTree('E'))
            System.out.println("Subtree rooted at E is perfect");
        else
            System.out.println("Subtree rooted at E is not perfect");
        System.out.println();
        
        tree.removeItem('D');
        System.out.println("D removed");  tree.printTreeInOrder();
        if(tree.isCompleteTree('E'))
            System.out.println("Subtree rooted at E is complete");
        else
            System.out.println("Subtree rooted at E is not complete");
        if(tree.isFullTree('E'))
            System.out.println("Subtree rooted at E is full");
        else
            System.out.println("Subtree rooted at E is not full");
        if(tree.isPerfectTree('E'))
            System.out.println("Subtree rooted at E is perfect");
        else
            System.out.println("Subtree rooted at E is not perfect");
        System.out.println();
        
        tree.removeItem('H');
        System.out.println("H removed");  tree.printTreeInOrder(); 
        tree.removeItem('C');
        System.out.println("C removed");  tree.printTreeInOrder();
        tree.removeItem('T');
        System.out.println("T removed");  tree.printTreeInOrder();
        tree.removeItem('S');
        System.out.println("S removed");  tree.printTreeInOrder();
        tree.removeItem('X');
        System.out.println("X removed");  tree.printTreeInOrder();
        tree.removeItem('E');
        System.out.println("E removed");  tree.printTreeInOrder();
        tree.removeItem('Y');
        System.out.println("Y removed");  tree.printTreeInOrder();
        tree.removeItem('W');
        System.out.println("W removed");  tree.printTreeInOrder();
        tree.removeItem('L');
        System.out.println("L removed");  tree.printTreeInOrder();
        tree.removeItem('I');
        System.out.println("I removed");  tree.printTreeInOrder();
        System.out.println();
        tree.removeItem('M');
        System.out.println("M removed");  tree.printTreeInOrder();    
        tree.printTreeInPreOrder();
        tree.printTreeInPostOrder();
        tree.printHeight();
        tree.printTreeInLevelOrder();
        if(tree.isCompleteTree('N'))
            System.out.println("Subtree rooted at N is complete");
        else
            System.out.println("Subtree rooted at N is not complete");
        if(tree.isFullTree('N'))
            System.out.println("Subtree rooted at N is full");
        else
            System.out.println("Subtree rooted at N is not full");
        if(tree.isPerfectTree('N'))
            System.out.println("Subtree rooted at N is perfect");
        else
            System.out.println("Subtree rooted at N is not perfect");
    }
}

    

