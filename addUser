#include <stdio.h>
#include <stdlib.h>
#include <string.h>

typedef struct User {
	int number;
	char name[10];
	int old;
	int sales;
} U;

int main(int argc, char *argv[]) {
	FILE *fp;
	U user;
	int people;
	fp = fopen("sales.txt", "a");
	
	printf("몇명의 사원을 등록하시겠습니까? : ");
	scanf("%d", &people);
	
	for(int i = 1; i <= people; i++){
		
		fprintf(fp, "=============== [%d번] ===============\n", i);
		
		printf("try -> %d 사원의 번호를 입력하세요. : ", i);
		scanf("%d", &user.number);
		fprintf(fp, "사원 번호: %d\n", user.number);
		
		printf("try -> %d 사원의 이름을 입력하세요. : ", i);
		scanf("%s", user.name);
		fprintf(fp, "사원 이름: %s\n", user.name);
		
		printf("try -> %d 사원의 나이를 입력하세요. : ", i);
		scanf("%d", &user.old);
		fprintf(fp, "사원 나이: %d\n", user.old);
		
		printf("try -> %d 사원의 월급을 입력하세요. : ", i);
		scanf("%d", &user.sales);
		fprintf(fp, "사원 월급: %d\n\n", user.sales);
		
	}
	printf("%d명의 사원의 정보를 추가했습니다.", people);
	fclose(fp);
	
	return 0;
}
