# System.Binary

```C#
namespace System.Buffers {
  public static class Binary {
    public static T Read<T>(this ReadOnlySpan<byte> buffer) where T : struct;
    public static T Read<T>(this Span<byte> buffer) where T : struct;
    public static short ReadInt16BigEndian(this ReadOnlySpan<byte> buffer);
    public static short ReadInt16BigEndian(this Span<byte> buffer);
    public static short ReadInt16LittleEndian(this ReadOnlySpan<byte> buffer);
    public static short ReadInt16LittleEndian(this Span<byte> buffer);
    public static int ReadInt32BigEndian(this ReadOnlySpan<byte> buffer);
    public static int ReadInt32BigEndian(this Span<byte> buffer);
    public static int ReadInt32LittleEndian(this ReadOnlySpan<byte> buffer);
    public static int ReadInt32LittleEndian(this Span<byte> buffer);
    public static long ReadInt64BigEndian(this ReadOnlySpan<byte> buffer);
    public static long ReadInt64BigEndian(this Span<byte> buffer);
    public static long ReadInt64LittleEndian(this ReadOnlySpan<byte> buffer);
    public static long ReadInt64LittleEndian(this Span<byte> buffer);
    public static ushort ReadUInt16BigEndian(this ReadOnlySpan<byte> buffer);
    public static ushort ReadUInt16BigEndian(this Span<byte> buffer);
    public static ushort ReadUInt16LittleEndian(this ReadOnlySpan<byte> buffer);
    public static ushort ReadUInt16LittleEndian(this Span<byte> buffer);
    public static uint ReadUInt32BigEndian(this ReadOnlySpan<byte> buffer);
    public static uint ReadUInt32BigEndian(this Span<byte> buffer);
    public static uint ReadUInt32LittleEndian(this ReadOnlySpan<byte> buffer);
    public static uint ReadUInt32LittleEndian(this Span<byte> buffer);
    public static ulong ReadUInt64BigEndian(this ReadOnlySpan<byte> buffer);
    public static ulong ReadUInt64BigEndian(this Span<byte> buffer);
    public static ulong ReadUInt64LittleEndian(this ReadOnlySpan<byte> buffer);
    public static ulong ReadUInt64LittleEndian(this Span<byte> buffer);
    public static byte Reverse(this byte value);
    public static short Reverse(this short value);
    public static int Reverse(this int value);
    public static long Reverse(this long value);
    public static sbyte Reverse(this sbyte value);
    public static ushort Reverse(this ushort value);
    public static uint Reverse(this uint value);
    public static ulong Reverse(this ulong value);
    public static bool TryRead<T>(this ReadOnlySpan<byte> buffer, out T value) where T : struct;
    public static bool TryRead<T>(this Span<byte> buffer, out T value) where T : struct;
    public static bool TryReadInt16BigEndian(this ReadOnlySpan<byte> buffer, out short value);
    public static bool TryReadInt16BigEndian(this Span<byte> buffer, out short value);
    public static bool TryReadInt16LittleEndian(this ReadOnlySpan<byte> buffer, out short value);
    public static bool TryReadInt16LittleEndian(this Span<byte> buffer, out short value);
    public static bool TryReadInt32BigEndian(this ReadOnlySpan<byte> buffer, out int value);
    public static bool TryReadInt32BigEndian(this Span<byte> buffer, out int value);
    public static bool TryReadInt32LittleEndian(this ReadOnlySpan<byte> buffer, out int value);
    public static bool TryReadInt32LittleEndian(this Span<byte> buffer, out int value);
    public static bool TryReadInt64BigEndian(this ReadOnlySpan<byte> buffer, out long value);
    public static bool TryReadInt64BigEndian(this Span<byte> buffer, out long value);
    public static bool TryReadInt64LittleEndian(this ReadOnlySpan<byte> buffer, out long value);
    public static bool TryReadInt64LittleEndian(this Span<byte> buffer, out long value);
    public static bool TryReadUInt16BigEndian(this ReadOnlySpan<byte> buffer, out ushort value);
    public static bool TryReadUInt16BigEndian(this Span<byte> buffer, out ushort value);
    public static bool TryReadUInt16LittleEndian(this ReadOnlySpan<byte> buffer, out ushort value);
    public static bool TryReadUInt16LittleEndian(this Span<byte> buffer, out ushort value);
    public static bool TryReadUInt32BigEndian(this ReadOnlySpan<byte> buffer, out uint value);
    public static bool TryReadUInt32BigEndian(this Span<byte> buffer, out uint value);
    public static bool TryReadUInt32LittleEndian(this ReadOnlySpan<byte> buffer, out uint value);
    public static bool TryReadUInt32LittleEndian(this Span<byte> buffer, out uint value);
    public static bool TryReadUInt64BigEndian(this ReadOnlySpan<byte> buffer, out ulong value);
    public static bool TryReadUInt64BigEndian(this Span<byte> buffer, out ulong value);
    public static bool TryReadUInt64LittleEndian(this ReadOnlySpan<byte> buffer, out ulong value);
    public static bool TryReadUInt64LittleEndian(this Span<byte> buffer, out ulong value);
    public static bool TryWrite<T>(this Span<byte> buffer, T value) where T : struct;
    public static bool TryWriteInt16BigEndian(this Span<byte> buffer, short value);
    public static bool TryWriteInt16LittleEndian(this Span<byte> buffer, short value);
    public static bool TryWriteInt32BigEndian(this Span<byte> buffer, int value);
    public static bool TryWriteInt32LittleEndian(this Span<byte> buffer, int value);
    public static bool TryWriteInt64BigEndian(this Span<byte> buffer, long value);
    public static bool TryWriteInt64LittleEndian(this Span<byte> buffer, long value);
    public static bool TryWriteUInt16BigEndian(this Span<byte> buffer, ushort value);
    public static bool TryWriteUInt16LittleEndian(this Span<byte> buffer, ushort value);
    public static bool TryWriteUInt32BigEndian(this Span<byte> buffer, uint value);
    public static bool TryWriteUInt32LittleEndian(this Span<byte> buffer, uint value);
    public static bool TryWriteUInt64BigEndian(this Span<byte> buffer, ulong value);
    public static bool TryWriteUInt64LittleEndian(this Span<byte> buffer, ulong value);
    public static void Write<T>(this Span<byte> buffer, T value) where T : struct;
    public static void WriteInt16BigEndian(this Span<byte> buffer, short value);
    public static void WriteInt16LittleEndian(this Span<byte> buffer, short value);
    public static void WriteInt32BigEndian(this Span<byte> buffer, int value);
    public static void WriteInt32LittleEndian(this Span<byte> buffer, int value);
    public static void WriteInt64BigEndian(this Span<byte> buffer, long value);
    public static void WriteInt64LittleEndian(this Span<byte> buffer, long value);
    public static void WriteUInt16BigEndian(this Span<byte> buffer, ushort value);
    public static void WriteUInt16LittleEndian(this Span<byte> buffer, ushort value);
    public static void WriteUInt32BigEndian(this Span<byte> buffer, uint value);
    public static void WriteUInt32LittleEndian(this Span<byte> buffer, uint value);
    public static void WriteUInt64BigEndian(this Span<byte> buffer, ulong value);
    public static void WriteUInt64LittleEndian(this Span<byte> buffer, ulong value);
  }
 }
```
