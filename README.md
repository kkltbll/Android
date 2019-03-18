@[TOC](这里写自定义目录标题)实验二 Android 布局

#利用线性布局实现代码如下：

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="wrap_content">
    <LinearLayout
        android:orientation="horizontal"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#000000">
    <Button
        android:id="@+id/btn_one"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:text="One,One"
        />

    <Button
        android:id="@+id/btn_two"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_weight="1.1"
        android:text="One,Two" />

    <Button
        android:id="@+id/btn_three"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_weight="1.1"
        android:text="One,Three" />

    <Button
        android:id="@+id/btn_four"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:text="One,Four" />
</LinearLayout>

    <LinearLayout
        android:orientation="horizontal"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#000000">
        <Button
            android:id="@+id/btn_five"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Two,One" />

        <Button
            android:id="@+id/btn_6"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Two,Two" />

        <Button
            android:id="@+id/btn_7"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.1"
            android:text="Two,Three" />

        <Button
            android:id="@+id/btn_8"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Two,Four" />
    </LinearLayout>
    <LinearLayout
        android:orientation="horizontal"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#000000">
        <Button
            android:id="@+id/btn_9"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.2"
            android:text="Three,One" />

        <Button
            android:id="@+id/btn_10"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.2"
            android:text="Three,Two" />

        <Button
            android:id="@+id/btn_11"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.2"
            android:text="Three,Three" />

        <Button
            android:id="@+id/btn_12"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.2"
            android:text="Three,Four"
            />
    </LinearLayout>
    <LinearLayout
        android:orientation="horizontal"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#000000">
        <Button
            android:id="@+id/btn_13"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Four,One" />

        <Button
            android:id="@+id/btn_14"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Four,Two" />

        <Button
            android:id="@+id/btn_15"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.1"
            android:textSize="12dp"
            android:text="Four,Three" />

        <Button
            android:id="@+id/btn_16"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:textSize="12dp"
            android:text="Four,Four"
            />
    </LinearLayout>

</LinearLayout>

##截图如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318200418639.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxNTg1ODAx,size_16,color_FFFFFF,t_70)

#利用ConstraintLayout实现源代码如下：

<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#ff0000"
        android:text="red"
        android:textColor="#000000"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#ff8247"
        android:text="orange"
        android:textColor="#000000"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="yellow"
        android:background="#fff000"
        android:textColor="#000000"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button7"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="30dp"
        android:layout_marginLeft="30dp"
        android:background="#b3ee3a"
        android:text="green"
        android:textColor="#000000"
        app:layout_constraintBaseline_toBaselineOf="@+id/button8"
        app:layout_constraintEnd_toStartOf="@+id/button8"
        app:layout_constraintHorizontal_chainStyle="packed"
        app:layout_constraintStart_toStartOf="parent" />

    <Button
        android:id="@+id/button8"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="30dp"
        android:background="#6495ED"
        android:text="blue"
        android:textColor="#000000"
        app:layout_constraintEnd_toStartOf="@+id/button9"
        app:layout_constraintStart_toEndOf="@+id/button7"
        app:layout_constraintTop_toBottomOf="@+id/button4" />

    <Button
        android:id="@+id/button9"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#4b0082"
        android:text="indigo"
        android:textColor="#000000"
        app:layout_constraintBaseline_toBaselineOf="@+id/button8"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/button8" />

    <Button
        android:id="@+id/button10"
        android:layout_width="599dp"
        android:layout_height="61dp"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="45dp"
        android:layout_marginEnd="8dp"
        android:layout_marginRight="8dp"
        android:text="violet"
        android:background="#BA55D3"
        android:textColor="#000000"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button7" />

</android.support.constraint.ConstraintLayout>

截图如下：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318200552699.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxNTg1ODAx,size_16,color_FFFFFF,t_70)

#利用表格布局实现代码如下：

<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1"
    android:background="#000000">

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Open..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-O"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>

    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save As..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-Shift-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <View
        android:layout_height="2dip"
        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Import..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Emport..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Ctrl-E"
            android:gravity="right"
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <View
        android:layout_height="2dip"

        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:textColor="#ffffff"
            android:text="Quit"
            android:padding="3dip"/>
    </TableRow>
</TableLayout>

截图如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318200704845.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxNTg1ODAx,size_16,color_FFFFFF,t_70)
