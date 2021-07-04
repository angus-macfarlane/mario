#include <stdio.h>
#include <cs50.h>
#include <string.h>

//void hashes(int height);
void better_hashes(int height);

int main(void)
{
    //Ask user for input, only accept values 1-8
    int height;
    do
    {
        height = get_int("Enter the height of your pyramid (1-8): \n");
    }
    while ((height < 1) || (height > 8));
    better_hashes(height);
}




//Print pyramind
void better_hashes(int height)
{
    char hash[9] = "#";
    int k = (height - 1); // used to calculate the number of spaces
    for (int i = 0; i < height; i++) // the loop adds a line, a hash, and removes a space each time it runs
    {
        if (i < (height - 1))
        {
            char add_hash[] = "#";
            printf("%*s%s", k, " ", hash);
            printf("%*s", 2, " ");
            printf("%s\n", hash);
            strcat(hash, add_hash);
            k--;
        }
        else // prints the bottom row without the first space
        {
            printf("%s", hash);
            printf("%*s", 2, " ");
            printf("%s\n", hash);
        }

    }
}
