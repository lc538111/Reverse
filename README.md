class Reverse
{
    public static void main(String[] args)
    {
        Scanner reader = new Scanner(System.in);
        System.out.println("Enter some Text!: ");
        String input = reader.next();
        char[] temparray = input.toCharArray();
        int left, right=0;
        right = temparray.length-1;
 
        for (left=0; left < right ; left++ ,right--)
        {
            // Swap values of left and right
            char temp = temparray[left];
            temparray[left] = temparray[right];
            temparray[right]=temp;
        }
 
        for (char c : temparray){
            System.out.print(c);
        System.out.println();
        }
    }
}
