https://www.udemy.com/course/unreal-engine-5-gas-top-down-rpg/learn/lecture/39782618#questions/21008736

![[{35AEC419-E1A7-42B0-9645-C021A4C38C27}.png]]
![[{0855EBAD-BAF7-4E46-BE2A-AC9155562E87}.png]]1. UPROPERTY(BlueprintReadOnly, ReplicatedUsing = OnRep_$NAME$, Category = "$CATEGORY$")
2. FGameplayAttributeData $NAME$;
3. ATTRIBUTE_ACCESSORS($CLASS$, $NAME$);

5. UFUNCTION()
6. virtual void OnRep_$NAME$(const FGameplayAttributeData& Old$NAME$)
7. {
8. GAMEPLAYATTRIBUTE_REPNOTIFY($CLASS$, $NAME$, Old$NAME$);
9. }

11. // TODO: Add the following line to the end of $CLASS$::GetLifetimeReplicatedProps():
12. // DOREPLIFETIME_CONDITION_NOTIFY($CLASS$, $NAME$, COND_None, REPNOTIFY_Always);