public class HanoiPuzzel{
    static void towerofHanoi(char source_rod , char destination_rod ,  char auxilary_rod , int n)
    {
        if(n==1)
        {
            System.out.println("Move disk from "u
                             +source_rod  +
                             " to "
                             +destination_rod);
        }
        else{
        towerofHanoi(source_rod,auxilary_rod,destination_rod,n-1);
        towerofHanoi(source_rod,destination_rod,auxilary_rod,1);
        towerofHanoi(auxilary_rod,destination_rod,source_rod,n-1);
        }
    }
        
            public static void main(String args[])
            {
                int noOfDisk = 4;
                towerofHanoi('A','B','C',noOfDisk);
            }
        


    
}

   
