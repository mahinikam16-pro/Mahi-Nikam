#include <stdio.h>
struct students{
int stu_roll_no;
char stu_name[20];
int stu_mar;
};
int main() {
int c;
struct students stu[100], sort;
int search_roll, found = 0;
int n=0;
while(1) {
printf("**************************************");
printf("\n ----Menu----\n1. Add records\n2. Display record\n3. sort\n4. search\n5. exit\n Enter your choice:");
scanf("%d",&c);

switch(c){
case 1:
printf("\n Enter No. of Students to add: ");
scanf("%d", &n);
for(int i =0;i<n;i++){
printf("\n**************************************\n");
printf("Enter Students Roll No.:");
scanf("%d",&stu[i].stu_roll_no);
printf("\nEnter Students Name:");
scanf("%s",stu[i].stu_name);
printf("\nEnter Students Marks:");
scanf("%d",&stu[i].stu_mar);
}
break;
case 2:
for(int i =0;i<n;i++){
printf("\n**************************************");
printf("\nStudents Roll No.: %d",stu[i].stu_roll_no);
printf("\nStudents Name: %s",stu[i].stu_name);
printf("\nStudents Marks: %d\n",stu[i].stu_mar);
}
break;
case 3:
for (int i = 0; i < n - 1; i++) {
for (int j = i + 1; j < n; j++) {
if (stu[i].stu_mar < stu[j].stu_mar) {
sort = stu[i];
stu[i] = stu[j];
stu[j] = sort;
}
}
}printf("\n**************************************"); 
printf("\n Record sorted\n Enter 2 to display sorted records\n");

break;
case 4:
printf("\n Enter Roll Number to search: ");
scanf("%d", &search_roll);
found = 0;
for (int i = 0; i < n; i++) {
if (stu[i].stu_roll_no == search_roll) {
printf("\n**************************************");
printf("\n--- Record Found ---\n");
printf("Students Roll No.: %d\n", stu[i].stu_roll_no);
printf("Students Name: %s\n", stu[i].stu_name);
printf("Students Marks: %d\n", stu[i].stu_mar);

found = 1;
break;
}
}
if (!found) {
printf("\nNo record found for Roll No.: %d\n", search_roll);
}
break;
case 5:
printf("\n Exiting program...\n");
return 0;
default:
printf("\nInvalid choice! Please try again.\n");
}
}
}
