# Grading-system-1
#include <stdio.h>
#include <stdlib.h>

void main()
{

   int Admission_number, coursework_marks;
    int Students_Name, Exam_marks;
    int sum;
    printf("Enter Admission number:");
    scanf("%d", &Admission_number);
    printf("Enter Students Name:");
    scanf("%s", &Students_Name);
    printf("Enter coursework marks:");
    scanf("%d", &coursework_marks);
    printf("Enter Exam marks:");
    scanf("%d", &Exam_marks);
    sum = coursework_marks + Exam_marks;
    if(sum<0 || sum>100)
    {
        printf("Wrong Entry");
    }
     else if(coursework_marks<15 | Exam_marks<15)
    {
        printf("Technical Fail");
    }
    else if(sum<40)
    {
        printf("Pass");
    }
    else if(sum<40)
    {
        printf("Grade F");
    }
    else if(sum>=40 && sum<50)
    {
        printf("Grade D");
    }
    else if(sum>=50 && sum<60)
    {
        printf("Grade C");
    }
    else if(sum>=60 && sum<70)
    {
        printf("Grade B");
    }
    else if(sum>=70 && sum<=100)
    {
        printf("Grade A");
    }

    return 0;
}
