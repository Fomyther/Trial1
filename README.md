some modifications about the code:

dataset.StudentID = dataset.StudentID.astype(int)

dataset.loc[dataset.score_Math.isnull(),['Pass_math']] = np.nan
dataset.loc[dataset.score_ELA.isnull(),['Pass_ELA']] = np.nan

change data type and remove warnings
