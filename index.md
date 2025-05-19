# Creating Headers the Github way
## This is an Header 2
### This is Header 3

![My Artwork](https://res.cloudinary.com/oyin-dawodu/image/upload/v1706637506/art/10.jpg)

```
export const getNotifications = createAsyncThunk(
    'auth/getNotifications',
    async (_, thunkAPI) => {
        try {
            const data = await authService.getNotifications()
            return data
        } catch (error) {
            const message = errorMessage(error)
            return thunkAPI.rejectWithValue(message)
        }
    },
)
```
