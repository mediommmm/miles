int main(void) {
	char cmd[255];
	memset(cmd, 0, 255);
	do
	{
		fgets(cmd, 255, stdin);
		cmd[strcspn ( cmd, "\n")] = '\0';
 
		
		if(!strcmp(cmd, "proceed"))
			printf("You may start.\n");
 
	} while(!strcmp(cmd, "leave"));	
	printf("Done!.");
	return 0;
}
